Yiistrap
========

[![Latest Stable Version](https://poser.pugx.org/crisu83/yiistrap/v/stable.png)](https://packagist.org/packages/crisu83/yiistrap)
[![Build Status](https://travis-ci.org/crisu83/yiistrap.svg?branch=bs3)](https://travis-ci.org/crisu83/yiistrap)

Twitter Bootstrap for Yii.

## Installation

The easiest way to install payment manager is to use Composer.
Add the following to your composer.json file:

```js
"require": {
	"crisu83/yiistrap": "dev-bs3"
}
````

Run the following command to download the extension:

```bash
php composer.phar update
```

Add the following to your application configuration:

```php
.....
'components' => array(
    .....
    'bootstrap' => array(
        'class' => '\TbApi',
    ),
),
.....
```

Add the following line to your main layout in protected/views/layouts/main.php to register the necessary CSS and JavaScript files:

```php
<?php Yii::app()->bootstrap->register(); ?>
```

If you are not using composer's autoload, then you need to add the following to your application configuration:

```php
'aliases' => array(
    'yiistrap' => __DIR__ . '/vendor/crisu83/yiistrap',
),
.....
'import' => array(
    .....
    'yiistrap.behaviors.*',
    'yiistrap.components.*',
    'yiistrap.form.*',
    'yiistrap.helpers.*',
    'yiistrap.widgets.*',
    .....
),
.....
```

## More

More documentation can be found here:
[http://www.getyiistrap.com](http://www.getyiistrap.com)
