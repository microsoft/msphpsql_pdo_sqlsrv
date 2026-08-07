# Microsoft Drivers for PHP for SQL Server — PDO_SQLSRV (PIE package)

This repository is the [PIE](https://github.com/php/pie) (PHP Installer for
Extensions) companion package for the **PDO_SQLSRV** driver, part of the
[Microsoft Drivers for PHP for SQL Server](https://github.com/microsoft/msphpsql).
PIE is the official replacement for PECL, which is now deprecated.

## Install

```sh
pie install microsoft/pdo_sqlsrv
```

`pdo_sqlsrv` builds on PHP's PDO extension, so PDO must be available (it ships
with PHP by default). PIE enforces this via the `ext-pdo` requirement.

> **Windows support (5.13.3+):** `pie install microsoft/pdo_sqlsrv` also works on
> Windows. PIE automatically downloads the matching pre-built DLL for your PHP
> version, thread-safety (TS/NTS), and architecture from this repository's GitHub
> release, so no manual DLL setup is required. For 5.13.2 and earlier, use the
> pre-built DLLs shipped with the
> [main driver releases](https://github.com/microsoft/msphpsql/releases) instead.

## Names at a glance

| Kind                         | Value                              |
| ---------------------------- | ---------------------------------- |
| GitHub repository            | `microsoft/msphpsql_pdo_sqlsrv`    |
| PIE / Composer package name  | `microsoft/pdo_sqlsrv`             |
| PHP extension name (php.ini) | `pdo_sqlsrv`                       |
| Install command              | `pie install microsoft/pdo_sqlsrv` |

## Requirements

- PHP 8.3 or newer
- PHP PDO extension (`ext-pdo`, bundled with PHP)
- Microsoft ODBC Driver for SQL Server (17 or 18)
- PIE 1.x (PIE itself requires PHP 8.1+ to run)

## Source code

The extension source is maintained in the main repository:
https://github.com/microsoft/msphpsql

This companion repository exists solely to publish the extension to Packagist/PIE;
its releases are kept in sync with the main driver releases.

## Documentation

https://learn.microsoft.com/sql/connect/php/microsoft-php-driver-for-sql-server

## Issues & support

Please report driver bugs and questions in the main repository:
https://github.com/microsoft/msphpsql/issues

Use this repository's issue tracker only for problems specific to the PIE /
Packagist package.

## License

MIT — see [LICENSE](LICENSE).
