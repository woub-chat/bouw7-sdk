# Swagger\Client\ApprovalApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteApprovalCriteria**](ApprovalApi.md#deleteApprovalCriteria) | **DELETE** /approval-template/criteria | Delete the given approval criteria.
[**deleteApprovalWorkflow**](ApprovalApi.md#deleteApprovalWorkflow) | **DELETE** /approval-template/workflow | Delete the given approval workflow.
[**findDefaultApprovalSettings**](ApprovalApi.md#findDefaultApprovalSettings) | **GET** /approval-template/default-settings | Find the default approval settings for the current organization.
[**findMatchingApprovalCriteria**](ApprovalApi.md#findMatchingApprovalCriteria) | **POST** /approval-template/match-criteria | Find the matching approval workflow based on the criteria with the highest score for the given schema.
[**getApprovalTemplateCriteria**](ApprovalApi.md#getApprovalTemplateCriteria) | **GET** /approval-template/criteria/{id} | Returns a single approval template criteria based on the given ID.
[**getApprovalTemplateWorkflow**](ApprovalApi.md#getApprovalTemplateWorkflow) | **GET** /approval-template/workflow/{id} | Returns a single approval template workflow based on the given ID, duplicate approvers are not filtered out!
[**getCriteriaTypes**](ApprovalApi.md#getCriteriaTypes) | **GET** /approval-template/criteria-types | Retrieve all approval template criteria types.
[**getWorkflowTypes**](ApprovalApi.md#getWorkflowTypes) | **GET** /approval-template/workflow-types | Retrieve all possible types with sub-types for an approval workflow.
[**listApprovalCriteria**](ApprovalApi.md#listApprovalCriteria) | **GET** /list/approval-template/criteria | Return a list of all approval criteria associated with the organization.
[**listApprovalWorkflows**](ApprovalApi.md#listApprovalWorkflows) | **GET** /list/approval-template/workflows | Returns a list of approval workflows for the organization of the current authenticated user. Use HQL to filter for specific items.
[**listPendingApprovalsAssignedToMe**](ApprovalApi.md#listPendingApprovalsAssignedToMe) | **GET** /list/approval/assigned-to-me | List all pending approvals for the current authenticated user.
[**postApprovalCriteria**](ApprovalApi.md#postApprovalCriteria) | **POST** /approval-template/criteria | Create or update the approval criteria with the schema.
[**postDefaultApprovalSettings**](ApprovalApi.md#postDefaultApprovalSettings) | **POST** /approval-template/default-settings | Update the default approval settings for the current organization.
[**postWorkflow**](ApprovalApi.md#postWorkflow) | **POST** /approval-template/workflow | Create or update the approval workflow with the schema.
[**voteOnContract**](ApprovalApi.md#voteOnContract) | **POST** /approval/{approval}/vote-on-contract | Vote on a contract approval.
[**voteOnPurchaseInvoice**](ApprovalApi.md#voteOnPurchaseInvoice) | **POST** /approval/{approval}/vote-on-purchase-invoice | Vote on a purchase invoice approval.


# **deleteApprovalCriteria**
> deleteApprovalCriteria($body)

Delete the given approval criteria.

Delete the given approval criteria.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedApprovalTemplateCriteria(); // \Swagger\Client\Model\CondensedApprovalTemplateCriteria | 

try {
    $apiInstance->deleteApprovalCriteria($body);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->deleteApprovalCriteria: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedApprovalTemplateCriteria**](../Model/CondensedApprovalTemplateCriteria.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteApprovalWorkflow**
> deleteApprovalWorkflow($body)

Delete the given approval workflow.

Delete the given approval workflow.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedApprovalTemplateWorkflow(); // \Swagger\Client\Model\CondensedApprovalTemplateWorkflow | 

try {
    $apiInstance->deleteApprovalWorkflow($body);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->deleteApprovalWorkflow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedApprovalTemplateWorkflow**](../Model/CondensedApprovalTemplateWorkflow.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findDefaultApprovalSettings**
> \Swagger\Client\Model\ApprovalTemplateSettings findDefaultApprovalSettings()

Find the default approval settings for the current organization.

Find the default approval settings.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->findDefaultApprovalSettings();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->findDefaultApprovalSettings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\ApprovalTemplateSettings**](../Model/ApprovalTemplateSettings.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findMatchingApprovalCriteria**
> \Swagger\Client\Model\ApprovalTemplateWorkflow findMatchingApprovalCriteria($body)

Find the matching approval workflow based on the criteria with the highest score for the given schema.

Match the criteria by the given schema and return the matching approval workflow or NULL if none can be found.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ApprovalTemplateCriteriaRequirements(); // \Swagger\Client\Model\ApprovalTemplateCriteriaRequirements | 

try {
    $result = $apiInstance->findMatchingApprovalCriteria($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->findMatchingApprovalCriteria: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ApprovalTemplateCriteriaRequirements**](../Model/ApprovalTemplateCriteriaRequirements.md)|  |

### Return type

[**\Swagger\Client\Model\ApprovalTemplateWorkflow**](../Model/ApprovalTemplateWorkflow.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getApprovalTemplateCriteria**
> \Swagger\Client\Model\ApprovalTemplateCriteria getApprovalTemplateCriteria($id)

Returns a single approval template criteria based on the given ID.

Returns a single approval template criteria based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getApprovalTemplateCriteria($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->getApprovalTemplateCriteria: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\ApprovalTemplateCriteria**](../Model/ApprovalTemplateCriteria.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getApprovalTemplateWorkflow**
> \Swagger\Client\Model\ApprovalTemplateWorkflow getApprovalTemplateWorkflow($id, $remove_duplicates, $project_id)

Returns a single approval template workflow based on the given ID, duplicate approvers are not filtered out!

Returns a single approval template workflow based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 
$remove_duplicates = true; // bool | 
$project_id = 56; // int | 

try {
    $result = $apiInstance->getApprovalTemplateWorkflow($id, $remove_duplicates, $project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->getApprovalTemplateWorkflow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **remove_duplicates** | **bool**|  | [optional]
 **project_id** | **int**|  | [optional]

### Return type

[**\Swagger\Client\Model\ApprovalTemplateWorkflow**](../Model/ApprovalTemplateWorkflow.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCriteriaTypes**
> object[] getCriteriaTypes()

Retrieve all approval template criteria types.

Retrieve all approval template criteria types.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getCriteriaTypes();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->getCriteriaTypes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object[]**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getWorkflowTypes**
> \Swagger\Client\Model\ApprovalTemplateWorkflowTypes[] getWorkflowTypes()

Retrieve all possible types with sub-types for an approval workflow.

Retrieve all possible types with sub-types for an approval workflow.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getWorkflowTypes();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->getWorkflowTypes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\ApprovalTemplateWorkflowTypes[]**](../Model/ApprovalTemplateWorkflowTypes.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listApprovalCriteria**
> \Swagger\Client\Model\ApprovalTemplateCriteriaList listApprovalCriteria($q)

Return a list of all approval criteria associated with the organization.

Return a list of approval criteria associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listApprovalCriteria($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->listApprovalCriteria: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\ApprovalTemplateCriteriaList**](../Model/ApprovalTemplateCriteriaList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listApprovalWorkflows**
> \Swagger\Client\Model\ApprovalTemplateWorkflowList listApprovalWorkflows($q)

Returns a list of approval workflows for the organization of the current authenticated user. Use HQL to filter for specific items.

Returns a list of approval workflows. Use HQL to filter for specific items.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listApprovalWorkflows($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->listApprovalWorkflows: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\ApprovalTemplateWorkflowList**](../Model/ApprovalTemplateWorkflowList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPendingApprovalsAssignedToMe**
> \Swagger\Client\Model\PendingApprovalList listPendingApprovalsAssignedToMe($q)

List all pending approvals for the current authenticated user.

List all pending approvals for the current authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listPendingApprovalsAssignedToMe($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->listPendingApprovalsAssignedToMe: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\PendingApprovalList**](../Model/PendingApprovalList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postApprovalCriteria**
> \Swagger\Client\Model\ApprovalTemplateCriteria postApprovalCriteria($body)

Create or update the approval criteria with the schema.

Create or update the approval criteria with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ApprovalTemplateCriteria(); // \Swagger\Client\Model\ApprovalTemplateCriteria | 

try {
    $result = $apiInstance->postApprovalCriteria($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->postApprovalCriteria: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ApprovalTemplateCriteria**](../Model/ApprovalTemplateCriteria.md)|  |

### Return type

[**\Swagger\Client\Model\ApprovalTemplateCriteria**](../Model/ApprovalTemplateCriteria.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postDefaultApprovalSettings**
> \Swagger\Client\Model\ApprovalTemplateSettings postDefaultApprovalSettings($body)

Update the default approval settings for the current organization.

Update the default approval settings.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ApprovalTemplateSettings(); // \Swagger\Client\Model\ApprovalTemplateSettings | 

try {
    $result = $apiInstance->postDefaultApprovalSettings($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->postDefaultApprovalSettings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ApprovalTemplateSettings**](../Model/ApprovalTemplateSettings.md)|  |

### Return type

[**\Swagger\Client\Model\ApprovalTemplateSettings**](../Model/ApprovalTemplateSettings.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postWorkflow**
> \Swagger\Client\Model\ApprovalTemplateWorkflow postWorkflow($body)

Create or update the approval workflow with the schema.

Create or update the approval workflow with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ApprovalTemplateWorkflow(); // \Swagger\Client\Model\ApprovalTemplateWorkflow | 

try {
    $result = $apiInstance->postWorkflow($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->postWorkflow: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ApprovalTemplateWorkflow**](../Model/ApprovalTemplateWorkflow.md)|  |

### Return type

[**\Swagger\Client\Model\ApprovalTemplateWorkflow**](../Model/ApprovalTemplateWorkflow.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **voteOnContract**
> voteOnContract($approval, $body)

Vote on a contract approval.

Approve or deny a contract approval.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$approval = 56; // int | Contract approval ID
$body = new \Swagger\Client\Model\ApprovalVote(); // \Swagger\Client\Model\ApprovalVote | 

try {
    $apiInstance->voteOnContract($approval, $body);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->voteOnContract: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **approval** | **int**| Contract approval ID |
 **body** | [**\Swagger\Client\Model\ApprovalVote**](../Model/ApprovalVote.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **voteOnPurchaseInvoice**
> voteOnPurchaseInvoice($approval, $body)

Vote on a purchase invoice approval.

Approve or deny a purchase invoice approval.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$approval = 56; // int | Purchase invoice approval ID
$body = new \Swagger\Client\Model\ApprovalVote(); // \Swagger\Client\Model\ApprovalVote | 

try {
    $apiInstance->voteOnPurchaseInvoice($approval, $body);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->voteOnPurchaseInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **approval** | **int**| Purchase invoice approval ID |
 **body** | [**\Swagger\Client\Model\ApprovalVote**](../Model/ApprovalVote.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

