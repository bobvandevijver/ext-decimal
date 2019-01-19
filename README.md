# PHP Decimal

[![Build Status](https://travis-ci.org/php-decimal/ext-decimal.svg?branch=master)](https://travis-ci.org/php-decimal/extension)
[![Build status](https://ci.appveyor.com/api/projects/status/lg5nw5tqgpmv1c33?svg=true)](https://ci.appveyor.com/project/rtheunissen/php-decimal)
[![PECL](https://img.shields.io/badge/PECL-1.1.0-blue.svg)](https://pecl.php.net/package/decimal)

Correctly-rounded, arbitrary precision decimal floating-point arithmetic in PHP 7.

## Documentation

See http://php-decimal.io

## Dependencies

- PHP 7
- [libmpdec 2.4](http://www.bytereef.org/mpdecimal/download.html)

```bash
sudo apt-get install libmpdec-dev
```

## Install

```
pecl install decimal
```

### Manual

```
git clone git@github.com:php-decimal/extension ext-decimal
cd ext-decimal

phpize
./configure
make
sudo make install
```

## Enable

You can do this temporarily using `php -dextension=decimal.so` or by adding `extension=decimal.so` to your INI. If you manage PHP with [phpbrew](https://github.com/phpbrew/phpbrew), you can use `phpbrew ext enable decimal`.

## Tests

```
php run-tests.php -P -q
```


TODO:
- EXPECTED/UNEXPECTED (go through existing first to confirm) (bench first!)
- Complete all comments, go through every single file. Search for all empty blocks
- Make sure that all methods are defined in the order that they are declared.
- Make sure that all methods have a test file.
- Do a spell check.
- Comparison and operations between builtins and Number implementations.
- Make sure that every file has a license doc comment.
- Make sure that every file is included in the package.xml info.
