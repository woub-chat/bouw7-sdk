# Swagger\Client\SecurityApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getProjectSecurityLink**](SecurityApi.md#getProjectSecurityLink) | **GET** /project/project-security-link/{id} | Returns a single project security link based on the given ID.
[**getSecurityObject**](SecurityApi.md#getSecurityObject) | **GET** /security-object/{id} | Returns a single security object based on the given ID.
[**postSecurityObject**](SecurityApi.md#postSecurityObject) | **POST** /security-object | Create or update the security object.


# **getProjectSecurityLink**
> \Swagger\Client\Model\ProjectSecurityLink getProjectSecurityLink($id)

Returns a single project security link based on the given ID.

Returns a single project security link based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SecurityApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Project security link ID.

try {
    $result = $apiInstance->getProjectSecurityLink($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SecurityApi->getProjectSecurityLink: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project security link ID. |

### Return type

[**\Swagger\Client\Model\ProjectSecurityLink**](../Model/ProjectSecurityLink.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSecurityObject**
> \Swagger\Client\Model\SecurityObject getSecurityObject($id)

Returns a single security object based on the given ID.

Returns a single security object based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SecurityApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Security object ID.

try {
    $result = $apiInstance->getSecurityObject($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SecurityApi->getSecurityObject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Security object ID. |

### Return type

[**\Swagger\Client\Model\SecurityObject**](../Model/SecurityObject.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postSecurityObject**
> \Swagger\Client\Model\SecurityObject postSecurityObject($body)

Create or update the security object.

Create or update a security object with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SecurityApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SecurityObject(); // \Swagger\Client\Model\SecurityObject | Security object.

try {
    $result = $apiInstance->postSecurityObject($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SecurityApi->postSecurityObject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SecurityObject**](../Model/SecurityObject.md)| Security object. |

### Return type

[**\Swagger\Client\Model\SecurityObject**](../Model/SecurityObject.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

