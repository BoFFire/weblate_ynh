<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Weblate for YunoHost

[![Integration level](https://dash.yunohost.org/integration/weblate.svg)](https://dash.yunohost.org/appci/app/weblate) ![](https://ci-apps.yunohost.org/ci/badges/weblate.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/weblate.maintain.svg)  
[![Install Weblate with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=weblate)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Weblate quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Weblate is a libre web-based translation tool with tight version control integration. It provides two user interfaces, propagation of translations across components, quality checks and automatic linking to source files.

**Shipped version:** 4.8~ynh1

**Demo:** https://hosted.weblate.org/

## Screenshots

![](./doc/screenshots/BigScreenshot.png)

## Disclaimers / important information

## GitHub

You'll need to give Weblate a GitHub user and a token. Please read [GitHub's documentation about token](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/).
This user will only be used to open the pull-request, each translation keep his author.

**SSH keys**, you will have to go in administration, and generate a public key for Weblate and add github.com so Weblate knows the fingerprint. Please note if your account already have a public key (ssh-rsa), you will have to manually add the Weblate's one to your GitHub account.

## Settings and upgrades

Almost everything related to Weblate's configuration is handled in a `settings.py` file.
You can edit the file `$final_path/local_settings.py` to enable or disable features.

# Miscellaneous

## LDAP connexion

It doesn't work yet, but while [it looks doable](https://docs.weblate.org/en/latest/admin/auth.html?highlight=LDAP#ldap-authentication), I'm unsure it is a good idea to connect this kind of tools to your LDAP.

## Documentation and resources

* Official app website: https://weblate.org
* Official user documentation: https://yunohost.org/apps
* Official admin documentation: https://docs.weblate.org/
* Upstream app code repository: https://github.com/WeblateOrg/weblate
* YunoHost documentation for this app: https://yunohost.org/app_weblate
* Report a bug: https://github.com/YunoHost-Apps/weblate_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/weblate_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/weblate_ynh/tree/testing --debug
or
sudo yunohost app upgrade weblate -u https://github.com/YunoHost-Apps/weblate_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps