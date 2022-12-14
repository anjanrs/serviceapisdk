# SwaggerClient-php
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0
- Build package: io.swagger.codegen.v3.generators.php.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/anjanrs/serviceapisdk.git"
    }
  ],
  "require": {
    "anjanrs/serviceapisdk": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 
$collection_id = "collection_id_example"; // string | 

try {
    $result = $apiInstance->getCollection($email, $collection_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getCollection: ', $e->getMessage(), PHP_EOL;
}


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 
$collection_id = 56; // int | 
$page = 56; // int | 
$recordsperpage = 56; // int | 

try {
    $result = $apiInstance->getCollectionDocs($email, $collection_id, $page, $recordsperpage);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getCollectionDocs: ', $e->getMessage(), PHP_EOL;
}


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 

try {
    $result = $apiInstance->getCollections($email);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getCollections: ', $e->getMessage(), PHP_EOL;
}


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 

try {
    $result = $apiInstance->getCompanyCollections($email);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getCompanyCollections: ', $e->getMessage(), PHP_EOL;
}


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 

try {
    $result = $apiInstance->getMyCollections($email);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getMyCollections: ', $e->getMessage(), PHP_EOL;
}


$apiInstance = new I2I\ServiceApi\Api\CollectionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$email = "email_example"; // string | 

try {
    $result = $apiInstance->getTags($email);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CollectionApi->getTags: ', $e->getMessage(), PHP_EOL;
}
?>
```

## Documentation for API Endpoints

All URIs are relative to */*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CollectionApi* | [**getCollection**](docs/Api/CollectionApi.md#getcollection) | **POST** /service/api/v1/collection | Get collection.
*CollectionApi* | [**getCollectionDocs**](docs/Api/CollectionApi.md#getcollectiondocs) | **POST** /service/api/v1/collectionDocs | Get documents under a collection
*CollectionApi* | [**getCollections**](docs/Api/CollectionApi.md#getcollections) | **POST** /service/api/v1/collections | Get collections
*CollectionApi* | [**getCompanyCollections**](docs/Api/CollectionApi.md#getcompanycollections) | **POST** /service/api/v1/companyCollections | Get company collections
*CollectionApi* | [**getMyCollections**](docs/Api/CollectionApi.md#getmycollections) | **POST** /service/api/v1/myCollections | Get my collections
*CollectionApi* | [**getTags**](docs/Api/CollectionApi.md#gettags) | **POST** /service/api/v1/tags | Get tags

## Documentation For Models

 - [Collection](docs/Model/Collection.md)
 - [CollectionData](docs/Model/CollectionData.md)
 - [CollectionDocVersion](docs/Model/CollectionDocVersion.md)
 - [CollectionDocs](docs/Model/CollectionDocs.md)
 - [CollectionDocsData](docs/Model/CollectionDocsData.md)
 - [Collections](docs/Model/Collections.md)
 - [CollectionsData](docs/Model/CollectionsData.md)
 - [Tags](docs/Model/Tags.md)
 - [TagsData](docs/Model/TagsData.md)
 - [Unauthorized](docs/Model/Unauthorized.md)
 - [V1CollectionBody](docs/Model/V1CollectionBody.md)
 - [V1CollectionDocsBody](docs/Model/V1CollectionDocsBody.md)
 - [V1CollectionsBody](docs/Model/V1CollectionsBody.md)
 - [V1CompanyCollectionsBody](docs/Model/V1CompanyCollectionsBody.md)
 - [V1MyCollectionsBody](docs/Model/V1MyCollectionsBody.md)
 - [V1TagsBody](docs/Model/V1TagsBody.md)

## Documentation For Authorization


## bearerAuth

- **Type**: HTTP bearer authentication


## Author



