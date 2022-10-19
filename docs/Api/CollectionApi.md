# I2I\ServiceApi\CollectionApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCollection**](CollectionApi.md#getcollection) | **POST** /service/api/v1/collection | Get collection.
[**getCollectionDocs**](CollectionApi.md#getcollectiondocs) | **POST** /service/api/v1/collectionDocs | Get documents under a collection
[**getCollections**](CollectionApi.md#getcollections) | **POST** /service/api/v1/collections | Get collections

# **getCollection**
> \I2I\ServiceApi\Model\Collection getCollection($email, $collection_id)

Get collection.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: bearerAuth
    $config = I2I\ServiceApi\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


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
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **string**|  | [optional]
 **collection_id** | **string**|  | [optional]

### Return type

[**\I2I\ServiceApi\Model\Collection**](../Model/Collection.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCollectionDocs**
> \I2I\ServiceApi\Model\CollectionDocs getCollectionDocs($email, $collection_id, $page, $recordsperpage)

Get documents under a collection

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: bearerAuth
    $config = I2I\ServiceApi\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


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
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **string**|  | [optional]
 **collection_id** | **int**|  | [optional]
 **page** | **int**|  | [optional]
 **recordsperpage** | **int**|  | [optional]

### Return type

[**\I2I\ServiceApi\Model\CollectionDocs**](../Model/CollectionDocs.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCollections**
> \I2I\ServiceApi\Model\Collections getCollections($email)

Get collections

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: bearerAuth
    $config = I2I\ServiceApi\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


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
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **string**|  | [optional]

### Return type

[**\I2I\ServiceApi\Model\Collections**](../Model/Collections.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

