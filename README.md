skype-status-php
================

PHP class to get Skype user's online status

## Usage

Instantiate SkypeStatus object
```php
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
