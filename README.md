<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Calckey for YunoHost

[![Integration level](https://dash.yunohost.org/integration/calckey.svg)](https://dash.yunohost.org/appci/app/calckey) ![Working status](https://ci-apps.yunohost.org/ci/badges/calckey.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/calckey.maintain.svg)
[![Install Calckey with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=calckey)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Calckey quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview


A greatly enhanced fork of Misskey with better UI/UX, security, features, and more! https://i.calckey.cloud/


    Calckey is based off of Misskey, a powerful microblogging server on ActivityPub with features such as emoji reactions, a customizable web UI, rich chatting, and much more!
    Calckey adds many quality of life changes and bug fixes for users and instance admins alike.
   


**Shipped version:** 13.1.1~ynh1

**Demo:** https://i.calckey.cloud/

## Screenshots

![Screenshot of Calckey](./doc/screenshots/screenshot-calckey.png)

## Disclaimers / important information

### Important points to read before installing

- *Calckey* requires a dedicated root domain, e.g. `Calckey.domain.tld`
- Due to Cypress dependency, *Calckey* only works on 64-bit CPU machines.
- *Calckey* can take quite some time to install (more then 30 minutes). So take out some time and grab yourself a coffee.
- If installing from command line, using `screen` is recommended to avoid disconnection. See below.
- After installation, first page can take time to load and may show timeout error. Give it time to make itself ready for you. Refresh the page after 2 or 3 minutes.
- The first account created will be an admin user and will have all the admin rights.

Using screen in case of disconnects

``` 
sudo apt-get install screen
screen
sudo yunohost app install https://github.com/YunoHost-Apps/Calckey_ynh.git
```
Recover after disconnect:
```
screen -d
screen -r
```

## Documentation and resources

* Official app website: <https://i.calckey.cloud/>
* Upstream app code repository: <https://codeberg.org/calckey/calckey>
* YunoHost documentation for this app: <https://yunohost.org/app_calckey>
* Report a bug: <https://github.com/YunoHost-Apps/calckey_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/calckey_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/calckey_ynh/tree/testing --debug
or
sudo yunohost app upgrade calckey -u https://github.com/YunoHost-Apps/calckey_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
