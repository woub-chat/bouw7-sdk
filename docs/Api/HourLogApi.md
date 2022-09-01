# Swagger\Client\HourLogApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getHourLogs**](HourLogApi.md#getHourLogs) | **GET** /project/{project}/hour-logs | Returns a list of hour logs associated with the given project.
[**listContactHourLogs**](HourLogApi.md#listContactHourLogs) | **GET** /list/hour-logs/contact | Returns a list of contact hour logs associated with your organization.
[**listEmployeeHourLogs**](HourLogApi.md#listEmployeeHourLogs) | **GET** /list/hour-logs/employee | Returns a list of employee hour logs associated with your organization.


# **getHourLogs**
> \Swagger\Client\Model\FilteredHourLogCollection getHourLogs($project, $q)

Returns a list of hour logs associated with the given project.

Returns a list of hour logs associated with the given project.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\HourLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID
$q = "q_example"; // string | Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language)

try {
    $result = $apiInstance->getHourLogs($project, $q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HourLogApi->getHourLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |
 **q** | **string**| Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) | [optional]

### Return type

[**\Swagger\Client\Model\FilteredHourLogCollection**](../Model/FilteredHourLogCollection.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listContactHourLogs**
> \Swagger\Client\Model\ContactHourLogList listContactHourLogs($q)

Returns a list of contact hour logs associated with your organization.

Returns a list of contact hour logs associated with your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\HourLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listContactHourLogs($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HourLogApi->listContactHourLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\ContactHourLogList**](../Model/ContactHourLogList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEmployeeHourLogs**
> \Swagger\Client\Model\EmployeeHourLogList listEmployeeHourLogs($q)

Returns a list of employee hour logs associated with your organization.

Returns a list of employee hour logs associated with your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\HourLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEmployeeHourLogs($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HourLogApi->listEmployeeHourLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EmployeeHourLogList**](../Model/EmployeeHourLogList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

