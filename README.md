# PHP class for communicating with DirectAdmin API
[![Latest Version](https://img.shields.io/github/release/solitweb/directadmin.svg?style=flat-square)](https://github.com/solitweb/directadmin/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/solitweb/directadmin/master.svg?style=flat-square)](https://travis-ci.org/solitweb/directadmin)
[![Total Downloads](https://img.shields.io/packagist/dt/solitweb/directadmin.svg?style=flat-square)](https://packagist.org/packages/solitweb/directadmin)

More info on the PHP class: http://forum.directadmin.com/showthread.php?t=258

## Installation

You can install this package via Composer using:

```bash
composer require solitweb/directadmin
```

## Usage

Basic usage. Get list of users owned by reseller:

```php
$api = new DirectAdmin;
$api->connect("domain", 2222);
$api->set_login("username", "password");
$api->set_method('GET');
$api->query("/CMD_API_SHOW_USERS");
$api->fetch_parsed_body();
print_r($api);
```

[More sample API scripts](http://files.directadmin.com/services/all/httpsocket/examples/)

## Credits
- [Phi1 'l0rdphi1' Stier](mailto:l0rdphi1@liquenox.net)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
