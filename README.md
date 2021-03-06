# NoCSRF, a simple PHP7 token class to prevent CSRF attacks.

[![Code Climate](https://codeclimate.com/github/JBlond/NoCSRF/badges/gpa.svg)](https://codeclimate.com/github/JBlond/NoCSRF) [![SensioLabsInsight](https://insight.sensiolabs.com/projects/9d4e9157-569c-46c3-b38c-0a3d00a923ff/mini.png)](https://insight.sensiolabs.com/projects/9d4e9157-569c-46c3-b38c-0a3d00a923ff)

* Author: Thibaut Despoulain
* Author: Mario
* Version: [![Latest Version](https://img.shields.io/github/release/JBlond/NoCSRF.svg?style=flat-square&label=Release)](https://github.com/JBlond/NoCSRF/releases)
* Licensed under the [MIT license](LICENSE.md)

## Usage 

For usage see the example/exmaple.php

## Public functions

- check
- enableOriginCheck
- generate

```PHP
<?php
$csfr = new jblond\Nocsrf;
$csfr->check('csrf_token', $_POST, $throwException = false, $time_span = null, $multiple = false);
$csfr->enableOriginCheck(); // optional
$csfr->generate( 'csrf_token' );
```
