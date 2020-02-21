# kk_library

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage

### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/krishnakumarkp/sdk-php.git"
    }
  ],
  "require": {
    "krishnakumarkp/sdk-php": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/kk_library/vendor/autoload.php');
```

## Tests

To run the unit tests:

```bash
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



// Configure Bearer (JWT) authorization: bearerAuth
$config = Person/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Person/Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->personGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->personGet: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://192.168.100.25/apikey_auth_jwt*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**personGet**](docs/Api/DefaultApi.md#personget) | **GET** /person | List all people
*DefaultApi* | [**personPost**](docs/Api/DefaultApi.md#personpost) | **POST** /person | Create a person


## Documentation For Models

 - [AuthError](docs/Model/AuthError.md)
 - [Error](docs/Model/Error.md)
 - [Person](docs/Model/Person.md)


## Documentation For Authorization



## bearerAuth


- **Type**: Bearer authentication (JWT)


## Author


