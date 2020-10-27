# PHP Coding Standard

The PHP coding standard of the Motionpicture projects. (temporary)

## Introduction

This project is [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) rules.
 It also contains the rules of the [Slevomat Coding Standard](https://github.com/slevomat/coding-standard).

## Installation

Standards can be installed with the [Composer](https://getcomposer.org/) dependency manager.

```bash
composer require --dev mp-okui/php-coding-standard
```

Make sure that the installed coding standards include **Motionpicture**.

```bash
phpcs -i
The installed coding standards are MySource, PEAR, PSR1, PSR12, PSR2, Squiz, Zend and Motionpicture
```

## Usage

### Command line

```bash
phpcs --standard=Motionpicture example.php
```

### Configuration File

If you need to further customize the selection of sniffs for your project - you can create a [custom ruleset file](https://github.com/squizlabs/PHP_CodeSniffer/wiki/Advanced-Usage#using-a-default-configuration-file).

```xml
<?xml version="1.0"?>
<ruleset name="MyStandard">
    <rule ref="Motionpicture"/>
</ruleset>
```
