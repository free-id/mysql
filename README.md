# MySQL parser

[![Latest Version on Packagist](https://img.shields.io/packagist/v/free-id/mysql.svg?style=flat-square)](https://packagist.org/packages/free-id/mysql)
[![Tests](https://github.com/free-id/mysql/actions/workflows/run-tests.yml/badge.svg?branch=main)](https://github.com/free-id/mysql/actions/workflows/run-tests.yml)
[![Total Downloads](https://img.shields.io/packagist/dt/free-id/mysql.svg?style=flat-square)](https://packagist.org/packages/free-id/mysql)

## Installation

You can install the package via composer:

```bash
composer require free-id/mysql
```

## Usage

```php
use FreeId\Mysql\Parser;

$parser = new Parser();
echo $parser->find();
```

## Parameters

| Parameter           | Description                                                                                                      | Default |
|---------------------|------------------------------------------------------------------------------------------------------------------|---------|
| host (string)       | IP address or database host name                                                                                 | -       |
| port (string)       | Database host port                                                                                               | -       |
| db (string)         | Name of the database to be searched                                                                              | -       |
| table (string)      | Name of the table in which the search will be performed                                                          | -       |
| credentials (array) | An associative array of credentials for connecting to the database with username and password keys, respectively | -       |
| column (string)     | The column to be searched by                                                                                     | id      |
| charset (string)    | Encoding                                                                                                         | utf8    |
| start_id (int)      | Identifier from which the search will start                                                                      | 1       |

## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](https://github.com/free-id/.github/blob/main/CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [Vitaly Kuzyaev](https://github.com/vitkuz573)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
