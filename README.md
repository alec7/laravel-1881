# Laravel Service Provider for 1881

Uses https://github.com/andersevenrud/1881 to set up a Service Provider for Laravel.

## Installation

```
composer require andersevenrud/laravel-1881
```

## Configuration

In `config/app.php`:

```

'providers' => [
    Laravel\DM1881\DM1881ServiceProvider::class,
],

'aliases' => [
  'DM1881' => Laravel\DM1881\Facades\DM1881::class
]
```

Then publish configurations:

```
$ php artisan vendor:publish
```

You now have `config/dm1881.php`.

## Usage

```
use DM1881;

function something() {

  $result = DM1881::searchPerson('ola bull');

}
```
## Changelog

* **1.0.1** - Updated composer.json
* **1.0.0** - Initial release

## License

MIT
