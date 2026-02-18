# Monolog

[![Build Status](https://github.com/Seldaek/monolog/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/Seldaek/monolog/actions)
[![Packagist Downloads](https://img.shields.io/packagist/dt/monolog/monolog.svg)](https://packagist.org/packages/monolog/monolog)
[![Latest Stable Version](https://img.shields.io/packagist/v/monolog/monolog.svg)](https://packagist.org/packages/monolog/monolog)
[![License](https://img.shields.io/packagist/l/monolog/monolog.svg)](LICENSE)

Sends your logs to files, sockets, inboxes, databases and various web services.

## Why use Monolog

- Wide collection of handlers for files, sockets, databases, webhooks and more.
- PSR-3 compatible: works with other PSR-3 consumers and libraries.
- Flexible formatters and processors to enrich or modify log records.
- Battle-tested in many frameworks and large projects.

## Requirements

- PHP >= 8.1

(See `composer.json` for full dependency and suggested extensions.)

## Quick Installation

Install the latest stable release via Composer:

```bash
composer require monolog/monolog
```

## Quick Usage

```php
<?php
use Monolog\Logger;
use Monolog\Handler\StreamHandler;
use Monolog\Level;

$log = new Logger('app');
$log->pushHandler(new StreamHandler('path/to/your.log', Level::Warning));

$log->warning('Something might be wrong');
$log->error('Something went wrong');
```

More examples and advanced usage are in the `doc/` directory.

## Documentation

- Usage: [doc/01-usage.md](doc/01-usage.md)
- Handlers, Formatters & Processors: [doc/02-handlers-formatters-processors.md](doc/02-handlers-formatters-processors.md)
- Utilities: [doc/03-utilities.md](doc/03-utilities.md)
- Extending Monolog: [doc/04-extending.md](doc/04-extending.md)
- Message structure: [message-structure.md](message-structure.md)

## Where to get help

- Issues and bug reports: https://github.com/Seldaek/monolog/issues
- Pull requests: https://github.com/Seldaek/monolog/pulls
- Discussions & Wiki: https://github.com/Seldaek/monolog/wiki

## Contributing

If you'd like to contribute, please open an issue or a pull request. For contribution guidelines, see `CONTRIBUTING.md` if present or the repository documentation.

## Maintainers

Primary maintainer: Jordi Boggiano (see contributors at https://github.com/Seldaek/monolog/contributors)

## License

Monolog is distributed under the MIT License — see [LICENSE](LICENSE) for details.

---

This file was generated from repository metadata. If you want me to replace the project `README.md` with this version, tell me and I will update it in-place.