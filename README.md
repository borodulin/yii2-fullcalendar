# FullCalendar widget for Yii2 framework

[![Latest Version](https://img.shields.io/packagist/v/conquer/fullcalendar.svg)](https://packagist.org/packages/conquer/fullcalendar)
[![Total Downloads](https://img.shields.io/packagist/dt/conquer/fullcalendar.svg)](https://packagist.org/packages/conquer/fullcalendar)
[![License](https://img.shields.io/packagist/l/conquer/fullcalendar.svg)](LICENSE.md)

## Description

FullCalendar is a jQuery plugin that provides a full-sized, drag & drop event calendar like the one below. It uses AJAX to fetch events on-the-fly and is easily configured to use your own feed format. It is visually customizable with a rich API.
For more information please visit [FullCalendar](http://fullcalendar.io/) 

## Requirements

- PHP 7.4 or 8.x
- Yii 2.0
- [asset-packagist](https://asset-packagist.org) repository configured in your application's `composer.json` (standard for Yii2 app templates)

## Installation

Install the extension via [Composer](https://getcomposer.org):

```bash
composer require conquer/fullcalendar:^1.1
```

## Usage

```php
use conquer\fullcalendar\FullCalendarWidget;

<?= FullCalendarWidget::widget([
    'weekends' => false
]); ?>

```

> **Security (1.1.0):** `events` are encoded as plain JSON, strings with the `js:` prefix in them are no longer
> turned into JavaScript, so event titles taken from users cannot inject code. Put callbacks into `options`.

## License

**conquer/fullcalendar** is released under the MIT License. See the bundled [`LICENSE.md`](LICENSE.md) for details.
