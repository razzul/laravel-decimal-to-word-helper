# laravel-decimal-to-word-helper
Convert decimals into word using custom helper in Laravel

> **Step 1: Copy the Helpers folder to your app folder**<br>
> **Step 2: Create an alias in config/app.php**

```php
<?php // Code within config/app.php

'aliases' => [
    ...
    'Helper' => 'App\Helpers\Helper::class',
    ...
```
> **Step 3: Use it in your Blade template**

```blade
{!! Helper::shout('this is how to use autoloading correctly!!') !!}
```
> **Also : Use this class anywhere in your Laravel app**

```php
<?php namespace App\Http\Controllers;
use App\Helpers\Helper;

class SomeController extends Controller
{
    public function __construct()
    {
        Helper::convert_number_to_words(123);
    }
    ...
```
