# php-proxy-app
Web Proxy Application built on php-proxy library ready to be installed on your server

## Installation

Keep in mind that this is a **project** and not a library. Installing this via *require* would do you not good.
A project such as this, should be installed straight into the public directory of your web server.

```bash
composer create-project athlon1600/php-proxy-app:dev-master /var/www/
```

If you do not have composer or trying to host this application on a **shared hosting**, then download a pre-installed version of this app from [**www.php-proxy.com**](https://www.php-proxy.com/)

## Keep it up-to-date

Application itself rarely will change, vast majority of changes will be done to its requirement packages like php-proxy. Simply call this command once in a while to make sure your proxy is always using the latest versions.

```
composer update
```

#### config.php

This file will be loaded into the global Config class.

#### /templates/

This is where we store all the "views"

### /plugins/

PHP-Proxy has many of its native plugins, but users are free to write their own which could then be loaded from this very folder. See /plugins/TestPlugin.php for an example.