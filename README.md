skype-status-php
================

[![Latest Stable Version](https://img.shields.io/packagist/v/Stichoza/skype-status-php.svg)](https://packagist.org/packages/stichoza/skype-status-php) [![Total Downloads](https://img.shields.io/packagist/dt/Stichoza/skype-status-php.svg)](https://packagist.org/packages/stichoza/skype-status-php) [![Downloads Month](https://img.shields.io/packagist/dm/Stichoza/skype-status-php.svg)](https://packagist.org/packages/stichoza/skype-status-php) [![License](https://img.shields.io/packagist/l/Stichoza/skype-status-php.svg)](https://packagist.org/packages/stichoza/skype-status-php) [![Code Climate](https://img.shields.io/codeclimate/github/Stichoza/skype-status-php.svg)](https://codeclimate.com/github/Stichoza/skype-status-php)

PHP class to get Skype user's online status
## Installation

Install this package through [Composer](https://getcomposer.org/). Edit your project's `composer.json` file to require `stichoza/skype-status-php`.

```json
"require": {
    "stichoza/skype-status-php": "~2.1"
}
```

**Or** run a command in your command line:

```
composer require stichoza/skype-status-php
```

## Usage

Instantiate SkypeStatus object
```php
use Stichoza\Skype\SkypeStatus;

$mySkype = new SkypeStatus("echo123");
```
Get online status code and/or string
```php
echo "User is " . $mySkype->getStatusString();    // output: User is online
echo "Status code: " . $mySkype->getStatusCode(); // output: Status code: 2
```

## Status Codes

 - **0** - Unknown
 - **1** - Offline
 - **2** - Online
 - **3** - Away
 - **4** - Unavailable
 - **5** - Do Not Disturb
 - **6** - Invisible
 - **7** - SkypeME
