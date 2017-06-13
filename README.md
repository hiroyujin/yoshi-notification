# Yoshi Notification
Library that helps to send notification to Yoshi application

## Basic usage
You must first configure the api key
```php
use YoshiNotification;

YoshiNotification::setApiKey("your api key");
```
Usage examples:
```php
use YoshiNotification;

$notification = new YoshiNotification();
$notification->send("Your notification");
```
Or
```php
use YoshiNotification;

YoshiNotification::send("Your notification");
```
Sending options
```php
use YoshiNotification;

YoshiNotification::send("Your notification",[
  'style' => 'info',
  'params' => [
    'custom_param_1' => 'Custom value'
    'custom_2' => 3232
  ]
]);
```

### Optional options
|Param        |Default          |Description              |
|:------------|:----------------|:------------------------|
|style        |primary          |style of your notification. Options: `primary`, `success`, `info`, `warning`, `danger` |
|params       |NULL             |array of your custom params       |
## Installation
just require the package using composer
```
composer require hiroyujin/yoshi-notification
```
