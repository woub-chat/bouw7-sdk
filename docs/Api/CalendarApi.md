# Swagger\Client\CalendarApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteDayOff**](CalendarApi.md#deleteDayOff) | **DELETE** /day-off | Delete the given day off.
[**deleteDayOffPerEmployee**](CalendarApi.md#deleteDayOffPerEmployee) | **DELETE** /organization/day-off-per-employee | Delete the given day off per employee.
[**getDayOff**](CalendarApi.md#getDayOff) | **GET** /day-off/{id} | Returns a single day off based on the given ID.
[**getDayOffPerEmployee**](CalendarApi.md#getDayOffPerEmployee) | **GET** /organization/day-off-per-employee/{id} | Returns a single day off per employee based on the given ID.
[**listDaysOff**](CalendarApi.md#listDaysOff) | **GET** /list/days-off | Returns a list of holidays / non-working days.
[**listDaysOffPerEmployee**](CalendarApi.md#listDaysOffPerEmployee) | **GET** /list/days-off-per-employee | Returns a list of day off per employee schemas associated with the organization.
[**postDayOff**](CalendarApi.md#postDayOff) | **POST** /day-off | Create or update the day off.
[**postDayOffPerEmployee**](CalendarApi.md#postDayOffPerEmployee) | **POST** /organization/day-off-per-employee | Create or update the day off per employee.


# **deleteDayOff**
> deleteDayOff($body)

Delete the given day off.

Delete the given day off.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DayOff(); // \Swagger\Client\Model\DayOff | 

try {
    $apiInstance->deleteDayOff($body);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->deleteDayOff: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DayOff**](../Model/DayOff.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDayOffPerEmployee**
> deleteDayOffPerEmployee($body)

Delete the given day off per employee.

Delete the given day off per employee.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DayOffPerEmployee(); // \Swagger\Client\Model\DayOffPerEmployee | 

try {
    $apiInstance->deleteDayOffPerEmployee($body);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->deleteDayOffPerEmployee: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DayOffPerEmployee**](../Model/DayOffPerEmployee.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDayOff**
> \Swagger\Client\Model\DayOff getDayOff($id)

Returns a single day off based on the given ID.

Returns a single DayOff based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getDayOff($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->getDayOff: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\DayOff**](../Model/DayOff.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDayOffPerEmployee**
> \Swagger\Client\Model\DayOffPerEmployee getDayOffPerEmployee($id)

Returns a single day off per employee based on the given ID.

Returns a single day off per employee based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getDayOffPerEmployee($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->getDayOffPerEmployee: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\DayOffPerEmployee**](../Model/DayOffPerEmployee.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listDaysOff**
> \Swagger\Client\Model\DayOffList listDaysOff($q)

Returns a list of holidays / non-working days.

Returns a list of holidays / non-working days.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Languae](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listDaysOff($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->listDaysOff: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Languae](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\DayOffList**](../Model/DayOffList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listDaysOffPerEmployee**
> \Swagger\Client\Model\DayOffPerEmployeeList listDaysOffPerEmployee($q)

Returns a list of day off per employee schemas associated with the organization.

Returns a list of days off per employee associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Languae](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listDaysOffPerEmployee($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->listDaysOffPerEmployee: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Languae](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\DayOffPerEmployeeList**](../Model/DayOffPerEmployeeList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postDayOff**
> \Swagger\Client\Model\DayOff postDayOff($body)

Create or update the day off.

Create or update a day off with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DayOff(); // \Swagger\Client\Model\DayOff | 

try {
    $result = $apiInstance->postDayOff($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->postDayOff: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DayOff**](../Model/DayOff.md)|  |

### Return type

[**\Swagger\Client\Model\DayOff**](../Model/DayOff.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postDayOffPerEmployee**
> \Swagger\Client\Model\DayOffPerEmployee postDayOffPerEmployee($body)

Create or update the day off per employee.

Create or update a day off per employee with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CalendarApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DayOffPerEmployee(); // \Swagger\Client\Model\DayOffPerEmployee | 

try {
    $result = $apiInstance->postDayOffPerEmployee($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CalendarApi->postDayOffPerEmployee: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DayOffPerEmployee**](../Model/DayOffPerEmployee.md)|  |

### Return type

[**\Swagger\Client\Model\DayOffPerEmployee**](../Model/DayOffPerEmployee.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

