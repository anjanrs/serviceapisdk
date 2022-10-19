# I2I\ServiceApi\CollectionApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCollections**](CollectionApi.md#getcollections) | **POST** /service/api/v1/collections | Get collections

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

