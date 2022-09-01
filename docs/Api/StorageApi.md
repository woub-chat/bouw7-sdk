# Swagger\Client\StorageApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteFile**](StorageApi.md#deleteFile) | **DELETE** /storage/file | Deletes a file associated with the given id.
[**downloadFile**](StorageApi.md#downloadFile) | **GET** /storage/{hash}/download | Returns the binary or base64 contents of a file.
[**getFileContents**](StorageApi.md#getFileContents) | **GET** /storage/{hash} | 
[**uploadFile**](StorageApi.md#uploadFile) | **POST** /storage/{modelType}/{modelId} | 


# **deleteFile**
> deleteFile($body)

Deletes a file associated with the given id.

Deletes a file associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\StorageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\File(); // \Swagger\Client\Model\File | 

try {
    $apiInstance->deleteFile($body);
} catch (Exception $e) {
    echo 'Exception when calling StorageApi->deleteFile: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\File**](../Model/File.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **downloadFile**
> \SplFileObject downloadFile($hash, $as_base64, $size)

Returns the binary or base64 contents of a file.

Returns the binary or base64 contents of a file.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\StorageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$hash = "hash_example"; // string | File URI
$as_base64 = true; // bool | Returns as base64
$size = 56; // int | Size of the thumbnail to serve (only if the file is an image)

try {
    $result = $apiInstance->downloadFile($hash, $as_base64, $size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StorageApi->downloadFile: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string**| File URI |
 **as_base64** | **bool**| Returns as base64 | [optional]
 **size** | **int**| Size of the thumbnail to serve (only if the file is an image) | [optional]

### Return type

[**\SplFileObject**](../Model/\SplFileObject.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getFileContents**
> string getFileContents($hash, $as_base64, $size)



Returns the contents of a file.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\StorageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$hash = "hash_example"; // string | File URI
$as_base64 = true; // bool | Returns as base64
$size = 56; // int | Size of the thumbnail to serve (only if the file is an image)

try {
    $result = $apiInstance->getFileContents($hash, $as_base64, $size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StorageApi->getFileContents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hash** | **string**| File URI |
 **as_base64** | **bool**| Returns as base64 | [optional]
 **size** | **int**| Size of the thumbnail to serve (only if the file is an image) | [optional]

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **uploadFile**
> \Swagger\Client\Model\File uploadFile($model_type, $model_id, $file)



Upload a file and associate it with a given entity.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\StorageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$model_type = "model_type_example"; // string | 
$model_id = 56; // int | 
$file = "/path/to/file.txt"; // \SplFileObject | 

try {
    $result = $apiInstance->uploadFile($model_type, $model_id, $file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StorageApi->uploadFile: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model_type** | **string**|  |
 **model_id** | **int**|  |
 **file** | **\SplFileObject**|  |

### Return type

[**\Swagger\Client\Model\File**](../Model/File.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

