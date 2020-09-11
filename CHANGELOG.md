commit 3293b627f4ebd71094352a334a820a39b7563560
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 02:18:57 2020 -0400

    Disabled Fedora testing
    
    Will come back to this later. Fedora support will address issue #11

commit fc685ad8aa5cf3ea67e9889206a4da7c77c5c1db
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 02:16:51 2020 -0400

    Added skip Ansible lint role name check

commit 69a9f60f2e950212ec598276adb16e6ef08637bc
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 02:16:26 2020 -0400

    Updated Ansible roles requirements

commit bfd04aec90ad4ef5fa67826d6e6ca5638e16fb86
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 02:15:50 2020 -0400

    Fixed Ubuntu 20.04 install
    
    Fixes #49

commit 33051c6bf351ff31e404977146bc8ab53fe679f3
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 01:50:52 2020 -0400

    Molecule tests updated
    
    All Molecule testing scenarios have been updated

commit 3b137d1dd7ada72ae0fe725ed492b32786eb62cc
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 01:48:19 2020 -0400

    Linting configs added
    
    - Ansible Lint
    - Flake8

commit 074ecfe95c26ab5d4aa9e4d050ac8f0767efb1f2
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 01:47:13 2020 -0400

    Python Requirements updated
    
    All prod/development Python requirements updated

commit 770a020914a8ccd8e86ff72a7c8044997bbd2bc7
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Sep 11 01:46:18 2020 -0400

    Updated CI tests
    
    The following CI tests have been updated:
    - GitLab CI
    - Travis CI
    - GitHub Actions

commit 06d64bb66479600e6201bfe36d6e56b065d07cc3
Author: Felix Bechstein <f@ub0r.de>
Date:   Tue May 26 15:46:16 2020 +0200

    fix install on EL8

commit 7af8e3e7b92e3c2978d9b3c6c9b5f52e0e6970c3
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sat Feb 22 00:43:52 2020 -0500

    Disabled Fedora testing
    
    - Issues that need to be addressed later

commit 698968e7017bbbc966ae1a2941d083ce2f1e0ab1
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sat Feb 22 00:07:52 2020 -0500

    Changed Molecule scenarios, tests, etc.

commit 28b89f420ed34d6dc2f7afdf1bdb5e834b954ef8
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sat Feb 22 00:06:36 2020 -0500

    Updated files, etc. after new structure

commit a8af449baae441aa7df3b97281413e6eea7cac4e
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Wed Feb 19 11:53:22 2020 -0500

    New files, etc. from cookiecutter template

commit 8f8e58d2f7249ee42488b6b4b3ccd4d334a7087e
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Wed Feb 19 11:52:36 2020 -0500

    Changes made based on new Molecule testing, etc.
    
    - When testing a few things were uncovered and have been addressed at
    this time.

commit 8ba792745746bc7ce0d7f07ab19b32ab20ea9829
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Wed Feb 19 11:51:28 2020 -0500

    Changes made based on implementing cookiecutter template

commit 691d32487e0d8e9c9d1952d0f73ec8865c7c6b67
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Wed Feb 19 00:34:35 2020 -0500

    Replaced previous Molecule testing with new

commit a6f810256600ea16589a697b6c08838a6be34106
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Mon Feb 10 16:54:12 2020 +0100

    Add client tls configuration for streams

commit 397a64b863c2d808b919512378a30640f73e02cb
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Tue Feb 11 09:48:52 2020 +0100

    force systemd for Ubuntu 16.04

commit 65b4fe5f83890e4dbc252594dad6983346f6b3d1
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Mon Feb 10 17:09:53 2020 +0100

    add missing dependencies

commit 436a8dbe694638d3fb46167f7833614b6b418821
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Mon Feb 10 18:28:47 2020 +0100

    CI: remove ubuntu 14.04 support reenable 16.04 support

commit 8ccc6040a722a919003560312b3ad6d426d6ca26
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Aug 1 08:02:54 2019 -0400

    Resolved formatting/task issues with Molecule testing
    
    - some services needed to be tweaked to account for sysvinit
    - linting issues were found and resolved

commit 01c046a3939bf586a2de6a51c7ded3a1314eeaba
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Aug 1 08:00:47 2019 -0400

    Added Molecule testing
    
    - Added Default (Docker) testing
    - Added vagrant (Vagrant) testing

commit d89c224662a82106e341532b7f43cdf2a857acdf
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Aug 1 07:59:35 2019 -0400

    Removed previous Travis testing methods

commit 5dfb9a50dd62e20dce76e04c57eb9287e58069fb
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Thu Jul 25 15:11:52 2019 +0200

    fix template logic for proxy

commit acb35c700fed298f0aad275bb15079e4435d0e4f
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Mon Jul 22 14:04:24 2019 +0200

    Feature: a netdata host can be defined as a proxy for streaming

commit 4e05065736e2ae6fb2caf629aadcfbde040d0741
Author: Alexandre Garand <alexandre.garand@fretlink.com>
Date:   Mon Jul 22 17:13:19 2019 +0200

    define variable to configure repeat frequency of alarms

commit d7b5c1ed16f78beae2783b29794856b1d8275cce
Author: Alexandre Garand <alexandre.garand@fretlink.com>
Date:   Tue Jul 23 11:09:21 2019 +0200

    replace blockinfile task by template task to manage health_alarm_notify.conf and add a variable to manage custom_sender_function

commit 39c397b456385d197222378faa53c09d3a7fd68a
Author: Paul B <paul@bonaud.fr>
Date:   Fri Jul 12 11:30:35 2019 +0200

    auto-update: don't break existing configurations

commit dbcc7a56df9f70594c83709ed43a411ade497b58
Author: Paul B <paul@bonaud.fr>
Date:   Thu Jul 11 18:00:59 2019 +0200

    auto-udpate: since Netdata v1.11 the auto-updater cron is automatic
    
    Netdata v1.11 now installs the cron by itself and the installer takes
    an `--auto-update` option to install the updater script.

commit 9f6ceff7f4304c3affcf6016b79d08b4d6c74290
Author: Markus Binsteiner <makkus@frkl.io>
Date:   Wed May 22 16:59:44 2019 +0200

    Fix for version check logic. did not work on Debian stretch.

commit 513be125f0515646a3d391b0c9c2cec1c20429c1
Author: Soumik <soumik@soumikghosh.com>
Date:   Wed Mar 13 10:09:15 2019 -0400

    Don't use a loop for installing pre-requisites

commit 61a0dbe347de54c3086f83363de73a0ac60f034a
Author: Soumik <soumik@soumikghosh.com>
Date:   Wed Dec 19 18:32:40 2018 -0500

    Make web mode configurable

commit 624f8167c6880b48faf6e6af2321e2ed331771ed
Author: Mickaël PERRIN <dev@mickaelperrin.fr>
Date:   Tue Dec 18 06:22:15 2018 +0100

    [BUGFIX] Notifications are not sent
    
    Missing permissions on /etc/netdata/health_alarm_notify.conf file

commit 21e1af7238e4419da98d24a30ac296563dbfe017
Author: bunchc <bunchc@gmail.com>
Date:   Mon Dec 10 10:42:33 2018 -0600

    Updating netdata git url to fix #23
    
    Netdata changed git URLs. This broke auto updating. Uninstalling netdata and reinstalling with the correct URL addresses this.
    
    This pull fixes #23

commit 375b546d1981908e2e4d19379746328d73965dda
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Wed Oct 10 11:33:50 2018 +0200

    Fix alarm configuration failing when file doesn't exists

commit 152ad798977348b251774f9dabe66420be803ca6
Author: John Hogenmiller <john@yourtech.us>
Date:   Tue Oct 9 08:38:37 2018 -0400

    Allow restart on failure
    
    This will cause the service to restart if it gets shut down uncleanly. It will wait 30 seconds between restart attempts

commit 7fe32b4392addde72cb7a0ebf1e2d5e35963af6f
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Mon Oct 8 17:59:31 2018 +0200

    really set netdata_hostname in backend and registry

commit b07e88495f23875707d9885563dfea1e379d9402
Author: Gaëtan Duchaussois <gaetan.duchaussois@fretlink.com>
Date:   Wed Oct 3 19:41:15 2018 +0200

    Allow hostname customisation

commit fd1724ae622dcd4225e1515e0de280d021e16e6a
Author: Guillaume Grussenmeyer <ggrussenmeyer@solent.fr>
Date:   Wed Aug 29 18:50:53 2018 +0200

    Added support for specifying master node port for streaming.

commit cdf12fa35fda8499512e286142313b106bd9f9a9
Author: Maxime Loliée <maxime@siliadev.com>
Date:   Fri Jul 27 11:23:58 2018 +0200

    Added some new parameters for tunning flood protection

commit 9d5d82db40ac80722d8c94d302e6db5815ec0e78
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 10:04:56 2018 -0400

    Resolved Ubuntu 18.04 install
    
    This resolves #12
    
    The iproute package no longer exists in Ubuntu 18.04 default
    installation so we needed to exclude installing this package only on
    Ubuntu 18.04+.

commit b2e0c932a534c637f284c91c9e7e4cf82e044062
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 01:04:28 2018 -0400

    Added Debian Stretch as supported distro

commit abe5dbfd6bef04107412637f56e01f554e5834b7
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 00:55:42 2018 -0400

    Disabled Fedora and Ubuntu 18.04 testing
    
    Fedora support is not available. Issue logged
    https://github.com/mrlesmithjr/ansible-netdata/issues/11
    
    Ubuntu Bionic(18.04) is failing by trying to install iproute which is
    not available. Issue logged for this
    https://github.com/mrlesmithjr/ansible-netdata/issues/12

commit 49333b4004be45718542d3bf3f6d9dd91cfd8e9d
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 00:41:09 2018 -0400

    Added build status

commit ec0964157a169daef106dc79b5542c7e581565a8
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 00:40:58 2018 -0400

    Added cron package as pre-req
    
    This package should exist anyways but to ensure that it is available we
    will install as a pre-req. This was discovered as testing with Travis-CI
    because cron is not installed in base container images.

commit 840ba74f3a2534cb064ea71afcab9181fea40227
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Apr 30 00:22:00 2018 -0400

    Implemented new Travis-CI testing

commit 049ca80f081b86ab348683f5b3b05fd52bdbe097
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sat Apr 14 22:27:34 2018 -0400

    Resolves #10

commit 5ed1ff2c63f91277e80bd0ee79f8c74099b4302b
Author: bunchc <bunchc@gmail.com>
Date:   Fri Apr 13 13:05:27 2018 -0500

    Adding configuration for netdata backends.
    * defaults/main.yml - added backend configuration variables
    * templates/netdata.conf.j2 - Added if/then logic around backend configuration

commit 1bbdd00354b3ee146c616d97c040290eec9fd212
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Mar 19 23:35:10 2018 -0400

    Create LICENSE

commit 2a6e440982728836db6dceddb53e7b45a3ae5ac6
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Mar 19 23:33:45 2018 -0400

    Split example playbook out into it's own file w/reference in README

commit 868f4f17e8f7584a25d12f64386c25a5f09aa365
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Mar 19 23:33:22 2018 -0400

    Cleaned up repo info and added TOC

commit b88d79cabf224af9067f2d2aa891e38584dc5584
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Mar 19 23:33:09 2018 -0400

    Cleaned up Ansible Galaxy meta info

commit fdad094eb31621faeac52e49e2d00527a32b0822
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Mar 19 23:32:49 2018 -0400

    Cleaned formatting of vars and tasks
    
    Removed single/double quotes where not needed to make code cleaner. Also
    changed single quotes to double quotes where they are needed.

commit 57e651426935598e7c40b1d93c2f323803f4c49c
Author: John H <john.hogenmiller@emc.com>
Date:   Wed Feb 21 11:29:32 2018 -0500

    Alarms customization

commit b452a5b75826c15c005eada11f4bc5d365f69495
Author: Sylvester Neau <neau@lemonde.fr>
Date:   Wed Jan 3 16:43:21 2018 +0100

    feat: add Netdata streaming configuration

commit 2023a45956fad6edfc03b441c0472f08a2c4eba5
Author: Chris <github.account@chrigel.net>
Date:   Mon Jan 29 21:00:05 2018 +0100

    Fix yaml syntax error.

commit c8a1b94391b50e3607b5668e5f04e08ba7431658
Author: Chris <github.account@chrigel.net>
Date:   Mon Jan 29 10:44:19 2018 +0100

    Removed restart handler from forced updater. The update script does that already.

commit 10df439ae354ae09602930c00721b20605eb27b6
Author: Chris <github.account@chrigel.net>
Date:   Mon Jan 29 10:40:27 2018 +0100

    Add forced update flag.

commit 01aaef8a28fb6c825216fb1fe84253bedc7c6723
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Apr 28 23:01:38 2017 -0400

    Added CentOS 6/7 functionality
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 13615487c89b40bf9db794d6142b6d68f9402ad3
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Apr 28 19:15:29 2017 -0400

    Removed reloading of systemd when using upstart
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 0ee4c8ee1fe94df91630b2e5d75aa91e66cfa6e4
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Apr 28 19:11:24 2017 -0400

    first commit
