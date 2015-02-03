oauth2
=============

[![Build Status](https://travis-ci.org/infusephp/oauth2.png?branch=master)](https://travis-ci.org/infusephp/oauth2)
[![Coverage Status](https://coveralls.io/repos/infusephp/oauth2/badge.png)](https://coveralls.io/r/infusephp/oauth2)
[![Latest Stable Version](https://poser.pugx.org/infuse/oauth2/v/stable.png)](https://packagist.org/packages/infuse/oauth2)
[![Total Downloads](https://poser.pugx.org/infuse/oauth2/downloads.png)](https://packagist.org/packages/infuse/oauth2)
[![HHVM Status](http://hhvm.h4cc.de/badge/infuse/oauth2.svg)](http://hhvm.h4cc.de/package/infuse/oauth2)

OAuth2 module for Infuse Framework

## Grant Types

Currently only these OAuth2 grant types are supported:
- Password (User Credentials)

## Response Type

The response type generated by the `POST /token` route is a [JWT](http://jwt.io) encoded access token.

## Installation

1. Install the package with [composer](http://getcomposer.org):

```
composer require infuse/oauth2
```

2. Generate the private key with: `openssl genrsa -out jwt_privkey.pem 2048`

3. Generate the public key with: `openssl rsa -in jwt_privkey.pem -pubout -out jwt_pubkey.pem`

The public and private key should each be stored in the base directory of your app.

## Acknowledgements

This project uses the awesome [oauth2-server-php](https://github.com/bshaffer/oauth2-server-php) library by Brent Shaffer.