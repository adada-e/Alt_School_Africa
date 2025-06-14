## Note, this file is written by cloud-init on first boot of an instance
## modifications made here will not survive a re-bundle.
## if you wish to make changes you can:
## a.) add 'apt_preserve_sources_list: true' to /etc/cloud/cloud.cfg
##     or do the same in user-data
## b.) add sources in /etc/apt/sources.list.d
## c.) make changes to template file /etc/cloud/templates/sources.list.tmpl

# See https://help.ubuntu.com/community/UpgradeNotes for how to upgrade to
# newer versions of the distribution.
deb https://archive.ubuntu.com/ubuntu focal main restricted
# deb-src https://archive.ubuntu.com/ubuntu focal main restricted

## Major bug fix updates produced after the final release of the
## distribution.
deb https://archive.ubuntu.com/ubuntu focal-updates main restricted
# deb-src https://archive.ubuntu.com/ubuntu focal-updates main restricted

## N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu
## team. Also, please note that software in universe WILL NOT receive any
## review or updates from the Ubuntu security team.
deb https://archive.ubuntu.com/ubuntu focal universe
# deb-src https://archive.ubuntu.com/ubuntu focal universe
deb https://archive.ubuntu.com/ubuntu focal-updates universe
# deb-src https://archive.ubuntu.com/ubuntu focal-updates universe

## N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu
## team, and may not be under a free licence. Please satisfy yourself as to
## your rights to use the software. Also, please note that software in
## multiverse WILL NOT receive any review or updates from the Ubuntu
## security team.
deb https://archive.ubuntu.com/ubuntu focal multiverse
# deb-src https://archive.ubuntu.com/ubuntu focal multiverse
deb https://archive.ubuntu.com/ubuntu focal-updates multiverse
# deb-src https://archive.ubuntu.com/ubuntu focal-updates multiverse

## N.B. software from this repository may not have been tested as
## extensively as that contained in the main release, although it includes
## newer versions of some applications which may provide useful features.
## Also, please note that software in backports WILL NOT receive any review
## or updates from the Ubuntu security team.
deb https://archive.ubuntu.com/ubuntu focal-backports main restricted universe multiverse
# deb-src https://archive.ubuntu.com/ubuntu focal-backports main restricted universe multiverse

## Uncomment the following two lines to add software from Canonical's
## 'partner' repository.
## This software is not part of Ubuntu, but is offered by Canonical and the
## respective vendors as a service to Ubuntu users.
# deb https://archive.canonical.com/ubuntu focal partner
# deb-src https://archive.canonical.com/ubuntu focal partner

deb https://security.ubuntu.com/ubuntu focal-security main restricted
# deb-src https://security.ubuntu.com/ubuntu focal-security main restricted
deb https://security.ubuntu.com/ubuntu focal-security universe
# deb-src https://security.ubuntu.com/ubuntu focal-security universe
deb https://security.ubuntu.com/ubuntu focal-security multiverse
# deb-src https://security.ubuntu.com/ubuntu focal-security multiverse

## PHP Version installed
PHP 7.4.3-4ubuntu2.29 (cli) (built: Mar 25 2025 18:57:03) ( NTS )
Copyright (c) The PHP Group
Zend Engine v3.4.0, Copyright (c) Zend Technologies
    with Zend OPcache v7.4.3-4ubuntu2.29, Copyright (c), by Zend Technologies