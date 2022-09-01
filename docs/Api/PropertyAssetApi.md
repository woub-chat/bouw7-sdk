# Swagger\Client\PropertyAssetApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deletePropertyAsset**](PropertyAssetApi.md#deletePropertyAsset) | **DELETE** /property-asset | Removes the given property asset.
[**getPropertyAsset**](PropertyAssetApi.md#getPropertyAsset) | **GET** /property-asset/{propertyAsset} | Returns a single property asset based on the given ID.
[**listPropertyAssets**](PropertyAssetApi.md#listPropertyAssets) | **GET** /list/property-assets | Returns a list of property assets associated with the organization.
[**postPropertyAsset**](PropertyAssetApi.md#postPropertyAsset) | **POST** /property-asset | Create or update a property asset with the data in the schema.


# **deletePropertyAsset**
> deletePropertyAsset($body)

Removes the given property asset.

Removes the given property asset.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PropertyAssetApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PropertyAsset(); // \Swagger\Client\Model\PropertyAsset | 

try {
    $apiInstance->deletePropertyAsset($body);
} catch (Exception $e) {
    echo 'Exception when calling PropertyAssetApi->deletePropertyAsset: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PropertyAsset**](../Model/PropertyAsset.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPropertyAsset**
> \Swagger\Client\Model\PropertyAsset getPropertyAsset($property_asset)

Returns a single property asset based on the given ID.

Returns a single property asset based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PropertyAssetApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$property_asset = 56; // int | 

try {
    $result = $apiInstance->getPropertyAsset($property_asset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PropertyAssetApi->getPropertyAsset: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **property_asset** | **int**|  |

### Return type

[**\Swagger\Client\Model\PropertyAsset**](../Model/PropertyAsset.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPropertyAssets**
> \Swagger\Client\Model\PropertyAssetList listPropertyAssets($q)

Returns a list of property assets associated with the organization.

Returns a list of property assets associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PropertyAssetApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listPropertyAssets($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PropertyAssetApi->listPropertyAssets: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\PropertyAssetList**](../Model/PropertyAssetList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postPropertyAsset**
> \Swagger\Client\Model\PropertyAsset postPropertyAsset($body)

Create or update a property asset with the data in the schema.

Create or update a property asset with the data in the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PropertyAssetApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PropertyAsset(); // \Swagger\Client\Model\PropertyAsset | 

try {
    $result = $apiInstance->postPropertyAsset($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PropertyAssetApi->postPropertyAsset: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PropertyAsset**](../Model/PropertyAsset.md)|  |

### Return type

[**\Swagger\Client\Model\PropertyAsset**](../Model/PropertyAsset.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

