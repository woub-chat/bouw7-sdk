# Swagger\Client\DepartmentApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteDepartment**](DepartmentApi.md#deleteDepartment) | **DELETE** /organization/department | Delete the given department.
[**deleteDepartmentWorkInProgressSettings**](DepartmentApi.md#deleteDepartmentWorkInProgressSettings) | **DELETE** /organization/department/work-in-progress-settings | Delete the given department work in progress settings.
[**getDepartment**](DepartmentApi.md#getDepartment) | **GET** /organization/department/{department} | Returns a single department based on the given ID.
[**postDepartment**](DepartmentApi.md#postDepartment) | **POST** /organization/department | Create or update the department with the schema.


# **deleteDepartment**
> deleteDepartment($body)

Delete the given department.

Delete the given department.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DepartmentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Department(); // \Swagger\Client\Model\Department | 

try {
    $apiInstance->deleteDepartment($body);
} catch (Exception $e) {
    echo 'Exception when calling DepartmentApi->deleteDepartment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Department**](../Model/Department.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDepartmentWorkInProgressSettings**
> deleteDepartmentWorkInProgressSettings($body)

Delete the given department work in progress settings.

Delete the given department work in progress settings.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DepartmentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedDepartmentWipSettings(); // \Swagger\Client\Model\CondensedDepartmentWipSettings | 

try {
    $apiInstance->deleteDepartmentWorkInProgressSettings($body);
} catch (Exception $e) {
    echo 'Exception when calling DepartmentApi->deleteDepartmentWorkInProgressSettings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedDepartmentWipSettings**](../Model/CondensedDepartmentWipSettings.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDepartment**
> \Swagger\Client\Model\Department getDepartment($department)

Returns a single department based on the given ID.

Returns a single department based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DepartmentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$department = 56; // int | 

try {
    $result = $apiInstance->getDepartment($department);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DepartmentApi->getDepartment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **department** | **int**|  |

### Return type

[**\Swagger\Client\Model\Department**](../Model/Department.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postDepartment**
> \Swagger\Client\Model\Department postDepartment($body)

Create or update the department with the schema.

Create or update a department with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DepartmentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Department(); // \Swagger\Client\Model\Department | 

try {
    $result = $apiInstance->postDepartment($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DepartmentApi->postDepartment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Department**](../Model/Department.md)|  |

### Return type

[**\Swagger\Client\Model\Department**](../Model/Department.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

