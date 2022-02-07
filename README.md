<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# SPIP for YunoHost

[![Integration level](https://dash.yunohost.org/integration/spip.svg)](https://dash.yunohost.org/appci/app/spip) ![](https://ci-apps.yunohost.org/ci/badges/spip.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/spip.maintain.svg)  
[![Install SPIP with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=spip)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install SPIP quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

CMS with a focus on collaborative edition and multilingualism

**Shipped version:** 4.0.1~ynh1

**Demo:** https://demo.spip.net/

## Disclaimers / important information

## Configuration

How to configure this app: by an admin panel.

#### Multi-users support

 * Are LDAP and HTTP auth supported? **Yes**
 * Can the app be used by multiple users? **Yes**

## Migrate from SPIP2

**This is not considered as stable yet, please do it with care and only for testing!**

This package handle the migration from SPIP2 to SPIP. For that, your
SPIP2 application must be **up-to-date** in YunoHost. To ensure that, execute:

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip2_ynh spip2 --debug
```

You will then have to upgrade your SPIP2 application with this repository.
This can only be done from the command-line interface - e.g. through SSH. Once you're connected, you simply have to execute the following:

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip_ynh spip2 --debug
```

The `--debug` option will let you see the full output. If you encounter any issue, please paste it.

Note that a cron job will be executed at some time after the end of this
command. You must wait that before doing any other application operations!
You should see that SPIP is installed after that.

## Documentation and resources

* Official app website: http://www.spip.net/
* Official user documentation: https://www.spip.net/en_rubrique57.html
* Official admin documentation: https://www.spip.net/en_rubrique209.html
* Upstream app code repository: https://git.spip.net/spip/spip
* YunoHost documentation for this app: https://yunohost.org/app_spip
* Report a bug: https://github.com/YunoHost-Apps/spip_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/spip_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
or
sudo yunohost app upgrade spip -u https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps