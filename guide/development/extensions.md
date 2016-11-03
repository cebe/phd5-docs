Packages (Extensions)
=====================

It is very easy to extend a phd-based application with existing composer packages. You can integrate any Yii2 extension or PHP library into phd.

```
docker-compose run --rm php bash
```

Finding packages
----------------

Start with a search on [Packagist](https://packagist.org) or from your command line

```
$ composer search -N "yii2-excel"
```

Installing packages
-------------------

To install an extension simply require it in your `composer.json` with the following command

```
$ composer require vendor/package
```

> Make sure to commit your `composer.lock` file, so your co-developers get the exact same version.

Configuring packages
--------------------

How to configure a package depends on the package and it's type. In general you can follow Yii's rules for application module and component configuration.

Show installed packages
-----------------------

```
$ composer show --installed
```
