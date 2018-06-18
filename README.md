Role Name
=========

An [Ansible] role to install/configure [Netdata]

Requirements
------------

Install required [Ansible] roles from `requirements.yml`

`ansible-galaxy install -r requirements.yml`

Role Variables
--------------

```yaml
---
# defaults file for ansible-netdata

# Defines info about enabling/scheduling auto updates for Netdata version
# https://github.com/firehol/netdata/wiki/Installation#auto-update
netdata_auto_updates:
  enabled: true
  day: '*'
  hour: '6'
  minute: '0'
  user: "root"
  weekday: '*'

# The IP address and port to listen to. This is a space separated list of
# IPv4 or IPv6 address and ports. The default will bind to all IP addresses
netdata_bind_to:
  - '*'

# Defines if Netdata should be configured
netdata_config: true

# Defines location of Netdata configuration file
netdata_config_file: '/etc/netdata/netdata.conf'
netdata_config_file: 'netdata.conf.j2'

# Defines pre-requisites for Debian systems
netdata_debian_pre_reqs:
  - 'autoconf-archive'
  - 'autoconf'
  - 'autogen'
  - 'automake'
  - 'build-essential'
  - 'curl'
  - 'gcc'
  - 'git'
  - 'iproute'
  - 'libmnl-dev'
  - 'libmnl0'
  - 'libuuid1'
  - 'lm-sensors'
  - 'make'
  - 'netcat'
  - 'pkg-config'
  - 'python-mysqldb'
  - 'python-psycopg2'
  - 'python-pymongo'
  - 'python-yaml'
  - 'util-linux'
  - 'uuid'
  - 'uuid-dev'
  - 'zlib1g-dev'

# Defines the Git repo to pull down for installs
netdata_git_repo: 'https://github.com/firehol/netdata.git'

# Defines whether Netdata health is enabled
netdata_health_enabled: true

# Defines if Netdata health alarms should be configured
netdata_alarm_configure: false

# Defines location of Netdata health_alarm_notify.conf
netdata_alarm_config_file: /etc/netdata/health_alarm_notify.conf

# Define configuration for health_alarm_notify.conf.
# Example:
# netdata_health_alarm_notify_configs:
#   - { key: https_proxy, value: http://localhost:3128 }
#   - { key: SLACK_WEBHOOK_URL, value: https://hooks.slack.com/ }
#   ...
netdata_alarm_notify_configs: {}

# Defines path to alarm-notify.sh
netdata_health_alarm_script: /usr/libexec/netdata/plugins.d/alarm-notify.sh

# The number of entries the netdata daemon will by default keep in memory
# for each chart dimension.
netdata_history: '3996'

# Defines Netdata installer script
netdata_installer: './netdata-installer.sh'

# When set to save netdata will save its round robin database on exit and
# load it on startup. When set to map the cache files will be updated in
# real time (check man mmap - do not set this on systems with heavy load or
# slow disks - the disks will continuously sync the in-memory database of
# netdata). When set to ram the round robin database will be temporary and it
# will be lost when netdata exits.
netdata_memory_mode: 'save'

# The default port to listen for web clients.
netdata_default_port: '19999'

# Defines pre-requisites for RedHat systems
netdata_redhat_pre_reqs:
  - 'autoconf'
  - 'automake'
  - 'curl'
  - 'gcc'
  - 'git'
  - 'iproute'
  - 'libmnl-devel'
  - 'libuuid-devel'
  - 'lm_sensors'
  - 'make'
  - 'MySQL-python'
  - 'nc'
  - 'pkgconfig'
  - 'python'
  - 'python-psycopg2'
  - 'PyYAML'
  - 'util-linux'
  - 'uuid'
  - 'uuid-devel'
  - 'zlib-devel'

# Defines if Netdata host should be enabled as a registry
# https://github.com/firehol/netdata/wiki/mynetdata-menu-item
netdata_registry_enabled: false

# https://registry.my-netdata.io
# https://github.com/firehol/netdata/wiki/mynetdata-menu-item
netdata_registry_to_announce: 'https://registry.my-netdata.io'

# Defines directory to store install source from Git repo
netdata_source_dir: '/usr/local/src/netdata'

# Defines if Netdata streaming should be configured
# https://github.com/firehol/netdata/wiki/Monitoring-ephemeral-nodes
netdata_stream_enabled: false

# Defines location of Netdata stream configuration file
netdata_stream_config_file: '/etc/netdata/stream.conf'
netdata_stream_config_file_template: 'stream.conf.j2'

# Defines Netdata API Key (must be generated with command uuidgen)
netdata_stream_api_key: '11111111-2222-3333-4444-555555555555'

# Defines Netdata master node
netdata_stream_master_node: ''

# Defines if Netdata should be uninstalled
# Caution: This does not prompt for uninstall as the original script
# was intended.
# https://github.com/firehol/netdata/wiki/Installation#uninstalling-netdata
netdata_uninstall: false

# Defines the Netdata uninstaller script
netdata_uninstaller: './netdata-uninstaller.sh'

# Defines if Netdata should be updated
# Not the same as auto_updates
netdata_update: false
# Force the update. Sometimes the update script skips installing new plugins.
netdata_update_force: false

# The frequency in seconds, for data collection
netdata_update_every: '1'

# Defines Netdata update script
netdata_updater: './netdata-updater.sh'

# Defines Netdata user info
netdata_user_info:
  group: 'netdata'
  user: 'netdata'
```

Dependencies
------------

Referenace [Requirements](#Requirements) section


Example Playbook
----------------

```yaml
---
- hosts: netdata_registry
  vars:
    netdata_registry_enabled: true
    netdata_registry_to_announce: 'http://192.168.250.10:{{ netdata_default_port }}'
    pri_domain_name: 'test.vagrant.local'
    netdata_stream_enabled: true
    netdata_stream_api_key: '11111111-2345-2345-2345-555555555555'
  roles:
    - role: ansible-nodejs
    - role: ansible-fail2ban
    - role: ansible-nginx
    - role: ansible-netdata
  tasks:

- hosts: netdata:!netdata_registry
  vars:
    netdata_registry_enabled: false
    netdata_registry_to_announce: 'http://192.168.250.10:{{ netdata_default_port }}'
    pri_domain_name: 'test.vagrant.local'
    netdata_stream_enabled: true
    netdata_stream_api_key: '11111111-2345-2345-2345-555555555555'
    netdata_stream_master_node: '192.168.250.10'
  roles:
    - role: ansible-nodejs
    - role: ansible-fail2ban
    - role: ansible-nginx
    - role: ansible-netdata
  tasks:
```

License
-------

BSD

Author Information
------------------


Larry Smith Jr.
- [@mrlesmithjr]
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com

[@mrlesmithjr]: <https://www.twitter.com/mrlesmithjr>

[Ansible]: <https://www.ansible.com>
[Netdata]: <https://my-netdata.io/>
