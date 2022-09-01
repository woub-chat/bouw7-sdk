# Swagger\Client\QuotationApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteQuotationReminder**](QuotationApi.md#deleteQuotationReminder) | **DELETE** /quotation/reminder | Deletes a quotation reminder associated with the given ID.
[**getQuotation**](QuotationApi.md#getQuotation) | **GET** /quotation/{quotation} | Returns the document of an existing quotation.
[**getQuotationReminder**](QuotationApi.md#getQuotationReminder) | **GET** /quotation/reminder/{quotationReminder} | Returns a quotation reminder based on the given ID.
[**listQuotationReminders**](QuotationApi.md#listQuotationReminders) | **GET** /list/quotation-reminders | Returns a list of quotation reminders associated with your organization.
[**listQuotationStatusLogs**](QuotationApi.md#listQuotationStatusLogs) | **GET** /list/quotation-status-logs | Returns a list of quotation status logs associated with any quotation for your organization.
[**listQuotations**](QuotationApi.md#listQuotations) | **GET** /list/quotations | Returns a list of quotations associated with your organization.
[**newQuotationForProject**](QuotationApi.md#newQuotationForProject) | **GET** /quotation/{project}/new | Returns the document with the project information filled in for a new quotation.
[**postQuotation**](QuotationApi.md#postQuotation) | **POST** /quotation | Creates or updates an quotation based on the given document.
[**postQuotationReminder**](QuotationApi.md#postQuotationReminder) | **POST** /quotation/reminder | Create or update the quotation reminder.


# **deleteQuotationReminder**
> deleteQuotationReminder($body)

Deletes a quotation reminder associated with the given ID.

Delete the given quotation reminder.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedQuotationReminder(); // \Swagger\Client\Model\CondensedQuotationReminder | 

try {
    $apiInstance->deleteQuotationReminder($body);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->deleteQuotationReminder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedQuotationReminder**](../Model/CondensedQuotationReminder.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getQuotation**
> \Swagger\Client\Model\Quotation getQuotation($quotation)

Returns the document of an existing quotation.

Returns the document of the given quotation.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quotation = 56; // int | Quotation ID

try {
    $result = $apiInstance->getQuotation($quotation);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->getQuotation: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotation** | **int**| Quotation ID |

### Return type

[**\Swagger\Client\Model\Quotation**](../Model/Quotation.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getQuotationReminder**
> \Swagger\Client\Model\QuotationReminder getQuotationReminder($quotation_reminder)

Returns a quotation reminder based on the given ID.

Returns a quotation reminder based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quotation_reminder = 56; // int | 

try {
    $result = $apiInstance->getQuotationReminder($quotation_reminder);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->getQuotationReminder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotation_reminder** | **int**|  |

### Return type

[**\Swagger\Client\Model\QuotationReminder**](../Model/QuotationReminder.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listQuotationReminders**
> \Swagger\Client\Model\QuotationReminderList listQuotationReminders($q)

Returns a list of quotation reminders associated with your organization.

Returns a list of quotation reminders associated with your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listQuotationReminders($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->listQuotationReminders: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\QuotationReminderList**](../Model/QuotationReminderList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listQuotationStatusLogs**
> \Swagger\Client\Model\QuotationStatusLogList listQuotationStatusLogs($q)

Returns a list of quotation status logs associated with any quotation for your organization.

Returns a list of quotation status logs associated with any quotation for your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listQuotationStatusLogs($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->listQuotationStatusLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\QuotationStatusLogList**](../Model/QuotationStatusLogList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listQuotations**
> \Swagger\Client\Model\QuotationList listQuotations($q)

Returns a list of quotations associated with your organization.

Returns a list of quotations associated with your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listQuotations($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->listQuotations: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\QuotationList**](../Model/QuotationList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **newQuotationForProject**
> \Swagger\Client\Model\Quotation newQuotationForProject($project)

Returns the document with the project information filled in for a new quotation.

Returns the document with the project information filled in for a new quotation.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID

try {
    $result = $apiInstance->newQuotationForProject($project);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->newQuotationForProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |

### Return type

[**\Swagger\Client\Model\Quotation**](../Model/Quotation.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postQuotation**
> \Swagger\Client\Model\Quotation postQuotation($quotation)

Creates or updates an quotation based on the given document.

Returns the document of the saved quotation.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quotation = new \Swagger\Client\Model\Quotation(); // \Swagger\Client\Model\Quotation | The quotation document to save.

try {
    $result = $apiInstance->postQuotation($quotation);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->postQuotation: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotation** | [**\Swagger\Client\Model\Quotation**](../Model/Quotation.md)| The quotation document to save. |

### Return type

[**\Swagger\Client\Model\Quotation**](../Model/Quotation.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postQuotationReminder**
> \Swagger\Client\Model\QuotationReminder postQuotationReminder($body)

Create or update the quotation reminder.

Create or update the quotation reminder with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\QuotationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\QuotationReminder(); // \Swagger\Client\Model\QuotationReminder | 

try {
    $result = $apiInstance->postQuotationReminder($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotationApi->postQuotationReminder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\QuotationReminder**](../Model/QuotationReminder.md)|  |

### Return type

[**\Swagger\Client\Model\QuotationReminder**](../Model/QuotationReminder.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

