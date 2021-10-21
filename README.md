SchildiChat For yunohost
=================

[![Integration level](https://dash.yunohost.org/integration/schildichat.svg)](https://dash.yunohost.org/appci/app/schildichat) ![](https://ci-apps.yunohost.org/ci/badges/schidichat.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/schildichat.maintain.svg)  
[![Install SchildiChat with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=schildichat)

> *This package allow you to install SchildiChat quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

Overview
--------

It's a webclient for matrix. For a matrix server you can install synapse on your server : https://github.com/YunoHost-Apps/synapse_ynh

Yunohost chatroom with matrix : [https://app.schildi.chat/#/room/#yunohost:matrix.org](https://app.schildi.chat/#/room/#yunohost:matrix.org)

**Shipped version:** 1.9.0-sc.1

Screenshots
-----------

#### Own your conversations

SchildiChat is a Matrix client based on Element with a more traditional instant messaging experience.

![](https://user-images.githubusercontent.com/42138517/138269694-20c544ea-9034-4f1f-af59-a1115192c213.png)

Demo
----

* [Official demo](https://app.schildi.chat)

Documentation
-------------

 * Official documentation: https://element.io/help
 * YunoHost documentation: There no other documentations, feel free to contribute.

YunoHost specific features
--------------------------

### Multi-users support

Now this application support the sso. If you want to use the sso you need to define the path to the default homeserver as your homeserver witch is installed on your yunohost instance.

### Supported architectures

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/schildichat%20%28Apps%29.svg)](https://ci-apps.yunohost.org/ci/apps/schildichat/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/schildichat%20%28Apps%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/schildichat/)

<!--## Limitations

* Any known limitations.-->

Additional informations
-----------------------

### Important Security Note

We do not recommend running SchildiChat from the same domain name as your Matrix
homeserver (synapse).  The reason is the risk of XSS (cross-site-scripting)
vulnerabilities that could occur if someone caused SchildiChat to load and render
malicious user generated content from a Matrix API which then had trusted
access to SchildiChat (or other apps) due to sharing the same domain.

We have put some coarse mitigations into place to try to protect against this
situation, but it's still not good practice to do it in the first place.  See
https://github.com/vector-im/riot-web/issues/1977 for more details.

Links
-----

 * Report a bug: https://github.com/benjaminwolkchen/schildichat_ynh/issues
 * App website: https://schildi.chat
 * YunoHost website: https://yunohost.org/

---

Install
-------

From command line:

`sudo yunohost app install -l schildichat https://github.com/benjaminwolkchen/schildichat_ynh`

Upgrade
-------

From command line:

`sudo yunohost app upgrade schildichat -u https://github.com/benjaminwolkchen/schildichat_ynh`

Developers infos
----------------

Please do your pull request to the [testing branch](https://github.com/benjaminwolkchen/schildichat_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/benjaminwolkchen/schildichat_ynh/tree/testing --debug
or
sudo yunohost app upgrade schildichat -u https://github.com/benjaminwolkchen/schildichat_ynh/tree/testing --debug
```

License
-------

SchildiChat-Web is published under the Apache License : https://github.com/SchildiChat/element-web/blob/sc/LICENSE

Todo for official App
---------------------

- Improve documentation
