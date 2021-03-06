
[uri_license]: http://www.gnu.org/licenses/agpl.html
[uri_license_image]: https://img.shields.io/badge/License-AGPL%20v3-blue.svg

[![License: AGPL v3][uri_license_image]][uri_license]
[![Build Status](https://travis-ci.org/Monogramm/docker-erpnext-poc_app_store.svg)](https://travis-ci.org/Monogramm/docker-erpnext-poc_app_store)
[![Docker Automated buid](https://img.shields.io/docker/cloud/build/monogramm/docker-erpnext-poc_app_store.svg)](https://hub.docker.com/r/monogramm/docker-erpnext-poc_app_store/)
[![Docker Pulls](https://img.shields.io/docker/pulls/monogramm/docker-erpnext-poc_app_store.svg)](https://hub.docker.com/r/monogramm/docker-erpnext-poc_app_store/)
[![](https://images.microbadger.com/badges/version/monogramm/docker-erpnext-poc_app_store.svg)](https://microbadger.com/images/monogramm/docker-erpnext-poc_app_store)
[![](https://images.microbadger.com/badges/image/monogramm/docker-erpnext-poc_app_store.svg)](https://microbadger.com/images/monogramm/docker-erpnext-poc_app_store)

# ERPNext Docker container extended with custom apps

Docker image for ERPNext with additionnal apps.

This image was inspired by several other containers developed by the community:
* [emadshaaban92/docker-compose-erpnext](https://github.com/emadshaaban92/docker-compose-erpnext/) / [BizzoTech/docker-erpnext](https://github.com/BizzoTech/docker-erpnext) for the "_simple_" docker-compose setup
* [donysukardi/docker-frappe](https://github.com/donysukardi/docker-frappe) for the alpine variant (actually the source for BizzoTech images)
* [pipech/erpnext-docker-debian](https://github.com/pipech/erpnext-docker-debian) for the complete setup of apps and sites

Additional apps:
* https://github.com/AminovE99/erpnext_app_store: POC of an application to list remote Frappe apps from https://github.com/Monogramm/erpnext_app_listing/ (possibly starting point of a real Frappe app store)

Check base image [Monogramm/docker-erpnext](https://github.com/Monogramm/docker-erpnext) and [Monogramm/docker-frappe](https://github.com/Monogramm/docker-frappe) for details.

:construction: **This image is still in development!**

## What is ERPNext ?

Open Source ERP built for the web.

> [erpnext.com](https://erpnext.com/)

> [github erpnext](https://github.com/frappe/erpnext)

## Supported tags

https://hub.docker.com/r/monogramm/docker-erpnext-poc_app_store/

* ERPNext develop branch
    - `develop-alpine` `develop`
    - `develop-debian` `develop-stretch`
    - `develop-debian-slim` `develop-stretch-slim`
* ERPNext 11
    - `11-alpine` `11` `alpine` `latest`
    - `11-debian` `debian` `11-stretch` `stretch`
    - `11-debian-slim` `debian-slim` `11-stretch-slim` `stretch-slim`
* ERPNext 10 (branch 10.x.x for latest bug fixes)
    - `10-alpine` `10`
    - `10-debian` `10-stretch`
    - `10-debian-slim` `10-stretch-slim`

# Questions / Issues
If you got any questions or problems using the image, please visit our [Github Repository](https://github.com/Monogramm/docker-erpnext-poc_app_store) and write an issue.  

# References

A list of a few issues encountered during the development of this container for future reference:
* ERPNext installs fails with Postgresql due to missing column
    * _Solution_: none so far...
    * _References_:
        * https://github.com/frappe/erpnext/issues/18028

