# Changelog

All notable changes to the **`microsoft/pdo_sqlsrv`** PIE / Packagist package are
documented in this file.

This companion package only re-packages the **PDO_SQLSRV** driver for
[PIE](https://github.com/php/pie); the driver source and its full change history
live in the main repository. For driver-level changes see the
[msphpsql CHANGELOG](https://github.com/microsoft/msphpsql/blob/dev/CHANGELOG.md).
This file records changes to the PIE packaging metadata only.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added

- Initial PIE packaging for `microsoft/pdo_sqlsrv`, installable with
  `pie install microsoft/pdo_sqlsrv` on Linux and macOS.
- `composer.json` (`type: php-ext`, extension `pdo_sqlsrv`, `priority: 20`,
  requires `ext-pdo`) using
  `download-url-method: ["pre-packaged-source"]`.
- Windows is excluded via `os-families-exclude` for this release; Windows users
  continue to use the pre-built DLLs from the main driver releases.
