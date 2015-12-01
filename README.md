# ComposerRequireChecker

A CLI tool to analyze composer dependencies and verify that no unknown symbols are used in the sources of a package.
This will prevent you from using "soft" dependencies that are not defined within your `composer.json` require section.

[![current version](https://img.shields.io/packagist/v/maglnet/composer-require-checker.svg?style=flat-square)](https://packagist.org/packages/maglnet/composer-require-checker)
[![Build Status](https://img.shields.io/travis/maglnet/ComposerRequireChecker.svg?style=flat-square)](https://travis-ci.org/maglnet/ComposerRequireChecker)
[![Dependency Status](https://www.versioneye.com/user/projects/565df3b9b6f5ff00380001ea/badge.svg?style=flat)](https://www.versioneye.com/user/projects/565df3b9b6f5ff00380001ea)

## Usage

Composer require checker is not supposed to be installed as part of your project dependencies.
Instead, please install it in a separate directory via:

```sh
composer create-project -s dev maglnet/composer-require-checker
```

You can then use it against any of the projects on your machine:

```sh
bin/composer-require-checker check /path/to/your/project/composer.json
```

## License

This package is made available under the [MIT LICENSE](LICENSE).

## Credits

This package was initially designed by [Marco Pivetta](https://github.com/ocramius) and [Matthias Glaub](https://github.com/maglnet).