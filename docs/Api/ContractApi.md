# Swagger\Client\ContractApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteContractOrderLine**](ContractApi.md#deleteContractOrderLine) | **DELETE** /project/{project}/contract-order-line | Delete the given contract order line.
[**deletePurchaseOrder**](ContractApi.md#deletePurchaseOrder) | **DELETE** /contracts/purchase-order | Delete the given purchase order contract.
[**deletePurchaseOrderContractTerm**](ContractApi.md#deletePurchaseOrderContractTerm) | **DELETE** /contracts/purchase-order/contract-term | Delete the given purchase order contract term.
[**deleteSubcontractor**](ContractApi.md#deleteSubcontractor) | **DELETE** /contracts/subcontractor | Delete the given subcontractor contract.
[**deleteSubcontractorContractTerm**](ContractApi.md#deleteSubcontractorContractTerm) | **DELETE** /contracts/subcontractor/contract-term | Delete the given subcontractor contract term.
[**getCalledReceiptBySubcontractorContract**](ContractApi.md#getCalledReceiptBySubcontractorContract) | **GET** /contracts/subcontractor/called-receipts/{id} | Returns a list of subcontractor contract called receipts associated with the given ID.
[**getCalledReceiptsByPurchaseOrderContract**](ContractApi.md#getCalledReceiptsByPurchaseOrderContract) | **GET** /contracts/purchase-order/called-receipts/{id} | Returns a list of purchase order contract called receipts associated with the given ID.
[**getFilesByPurchaseOrderContract**](ContractApi.md#getFilesByPurchaseOrderContract) | **GET** /contracts/purchase-order/files/{id} | Returns a collection of purchase order contract files with the given ID.
[**getFilesBySubcontractorContract**](ContractApi.md#getFilesBySubcontractorContract) | **GET** /contracts/subcontractor/files/{id} | Returns a collection of subcontractor contract files with the given ID.
[**getPurchaseOrder**](ContractApi.md#getPurchaseOrder) | **GET** /contracts/purchase-order/{id} | Returns a single purchase order contract based on the given ID.
[**getPurchaseOrderContractHistoryEntries**](ContractApi.md#getPurchaseOrderContractHistoryEntries) | **GET** /contracts/purchase-order/log-entries/{id} | Returns a list of purchase order contract history entries associated with the given ID.
[**getPurchaseOrderCostTypes**](ContractApi.md#getPurchaseOrderCostTypes) | **GET** /contracts/purchase-order/cost-types | Returns available cost types for a purchase order.
[**getPurchaseOrderStatuses**](ContractApi.md#getPurchaseOrderStatuses) | **GET** /contracts/purchase-order/statuses | Returns available statuses for a purchase order.
[**getSubcontractor**](ContractApi.md#getSubcontractor) | **GET** /contracts/subcontractor/{id} | Returns a single subcontractor contract based on the given ID.
[**getSubcontractorContractHistoryEntries**](ContractApi.md#getSubcontractorContractHistoryEntries) | **GET** /contracts/subcontractor/log-entries/{id} | Returns a list of subcontractor contract history entries associated with the given ID.
[**getSubcontractorStatuses**](ContractApi.md#getSubcontractorStatuses) | **GET** /contracts/subcontractor/statuses | Returns available statuses for a subcontractor contract.
[**listContractOrderLines**](ContractApi.md#listContractOrderLines) | **GET** /list/contract-order-lines | Returns all contract order lines for the current organization. Use HQL to filter for specific items.
[**listPurchaseOrderContractTerms**](ContractApi.md#listPurchaseOrderContractTerms) | **GET** /list/purchase-order-contract-terms | Returns a list of purchase order contract terms.
[**listPurchaseOrderContracts**](ContractApi.md#listPurchaseOrderContracts) | **GET** /list/purchase-order-contracts | Returns a list of purchase order contracts.
[**listSubcontractorContractTerms**](ContractApi.md#listSubcontractorContractTerms) | **GET** /list/subcontractor-contract-terms | Returns a list of subcontractor contract terms.
[**listSubcontractorContracts**](ContractApi.md#listSubcontractorContracts) | **GET** /list/subcontractor-contracts | Returns a list of subcontractor contracts.
[**postContractOrderLine**](ContractApi.md#postContractOrderLine) | **POST** /project/{project}/contract-order-line | Create or update the contract order line.
[**postPurchaseOrder**](ContractApi.md#postPurchaseOrder) | **POST** /contracts/purchase-order | Create or update a purchase order contract with the schema.
[**postPurchaseOrderContractTerm**](ContractApi.md#postPurchaseOrderContractTerm) | **POST** /contracts/purchase-order/contract-term | Create or update the purchase order contract term.
[**postSubcontractor**](ContractApi.md#postSubcontractor) | **POST** /contracts/subcontractor | Create or update a subcontractor contract with the schema.
[**postSubcontractorContractTerm**](ContractApi.md#postSubcontractorContractTerm) | **POST** /contracts/subcontract/contract-term | Create or update the subcontractor contract term.
[**updatePurchaseOrderStatus**](ContractApi.md#updatePurchaseOrderStatus) | **PUT** /contracts/purchase-order/{id}/update-status/{status} | Update the purchase order contract with the given status.
[**updateSubcontractorStatus**](ContractApi.md#updateSubcontractorStatus) | **PUT** /contracts/subcontractor/{id}/update-status/{status} | Update the subcontractor contract with the given status.


# **deleteContractOrderLine**
> deleteContractOrderLine($body, $project)

Delete the given contract order line.

Delete the given contract order line.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedContractOrderLine(); // \Swagger\Client\Model\CondensedContractOrderLine | 
$project = "project_example"; // string | 

try {
    $apiInstance->deleteContractOrderLine($body, $project);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->deleteContractOrderLine: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedContractOrderLine**](../Model/CondensedContractOrderLine.md)|  |
 **project** | **string**|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deletePurchaseOrder**
> deletePurchaseOrder($body)

Delete the given purchase order contract.

Delete the given purchase order contract.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PurchaseOrderContract(); // \Swagger\Client\Model\PurchaseOrderContract | 

try {
    $apiInstance->deletePurchaseOrder($body);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->deletePurchaseOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PurchaseOrderContract**](../Model/PurchaseOrderContract.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deletePurchaseOrderContractTerm**
> deletePurchaseOrderContractTerm($body)

Delete the given purchase order contract term.

Delete the given purchase order contract term.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ContractTerm(); // \Swagger\Client\Model\ContractTerm | 

try {
    $apiInstance->deletePurchaseOrderContractTerm($body);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->deletePurchaseOrderContractTerm: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteSubcontractor**
> deleteSubcontractor($body)

Delete the given subcontractor contract.

Delete the given subcontractor contract.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SubcontractorContract(); // \Swagger\Client\Model\SubcontractorContract | 

try {
    $apiInstance->deleteSubcontractor($body);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->deleteSubcontractor: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SubcontractorContract**](../Model/SubcontractorContract.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteSubcontractorContractTerm**
> deleteSubcontractorContractTerm($body)

Delete the given subcontractor contract term.

Delete the given subcontractor contract term.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ContractTerm(); // \Swagger\Client\Model\ContractTerm | 

try {
    $apiInstance->deleteSubcontractorContractTerm($body);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->deleteSubcontractorContractTerm: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCalledReceiptBySubcontractorContract**
> \Swagger\Client\Model\CalledReceipt[] getCalledReceiptBySubcontractorContract($id)

Returns a list of subcontractor contract called receipts associated with the given ID.

Returns a list of subcontractor contract called receipts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Subcontractor contract ID

try {
    $result = $apiInstance->getCalledReceiptBySubcontractorContract($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getCalledReceiptBySubcontractorContract: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Subcontractor contract ID |

### Return type

[**\Swagger\Client\Model\CalledReceipt[]**](../Model/CalledReceipt.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCalledReceiptsByPurchaseOrderContract**
> \Swagger\Client\Model\CalledReceipt[] getCalledReceiptsByPurchaseOrderContract($id)

Returns a list of purchase order contract called receipts associated with the given ID.

Returns a list of purchase order contract called receipts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Purchase order contract ID

try {
    $result = $apiInstance->getCalledReceiptsByPurchaseOrderContract($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getCalledReceiptsByPurchaseOrderContract: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Purchase order contract ID |

### Return type

[**\Swagger\Client\Model\CalledReceipt[]**](../Model/CalledReceipt.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getFilesByPurchaseOrderContract**
> \Swagger\Client\Model\File[] getFilesByPurchaseOrderContract($id)

Returns a collection of purchase order contract files with the given ID.

Returns a collection of purchase order contract files.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Purchase order contract ID

try {
    $result = $apiInstance->getFilesByPurchaseOrderContract($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getFilesByPurchaseOrderContract: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Purchase order contract ID |

### Return type

[**\Swagger\Client\Model\File[]**](../Model/File.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getFilesBySubcontractorContract**
> \Swagger\Client\Model\File[] getFilesBySubcontractorContract($id)

Returns a collection of subcontractor contract files with the given ID.

Returns a collection of subcontractor contract files.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Subcontractor contract ID

try {
    $result = $apiInstance->getFilesBySubcontractorContract($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getFilesBySubcontractorContract: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Subcontractor contract ID |

### Return type

[**\Swagger\Client\Model\File[]**](../Model/File.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseOrder**
> \Swagger\Client\Model\PurchaseOrderContract getPurchaseOrder($id)

Returns a single purchase order contract based on the given ID.

Returns a single purchase order contract based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getPurchaseOrder($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getPurchaseOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\PurchaseOrderContract**](../Model/PurchaseOrderContract.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseOrderContractHistoryEntries**
> \Swagger\Client\Model\PurchaseOrderContractHistory[] getPurchaseOrderContractHistoryEntries($id)

Returns a list of purchase order contract history entries associated with the given ID.

Returns a list of purchase order contract history entries.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Purchase order contract ID

try {
    $result = $apiInstance->getPurchaseOrderContractHistoryEntries($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getPurchaseOrderContractHistoryEntries: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Purchase order contract ID |

### Return type

[**\Swagger\Client\Model\PurchaseOrderContractHistory[]**](../Model/PurchaseOrderContractHistory.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseOrderCostTypes**
> object[] getPurchaseOrderCostTypes()

Returns available cost types for a purchase order.

Returns available cost types for a purchase order.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getPurchaseOrderCostTypes();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getPurchaseOrderCostTypes: ', $e->getMessage(), PHP_EOL;
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

# **getPurchaseOrderStatuses**
> object[] getPurchaseOrderStatuses()

Returns available statuses for a purchase order.

Returns available statuses for a purchase order.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getPurchaseOrderStatuses();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getPurchaseOrderStatuses: ', $e->getMessage(), PHP_EOL;
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

# **getSubcontractor**
> \Swagger\Client\Model\SubcontractorContract getSubcontractor($id)

Returns a single subcontractor contract based on the given ID.

Returns a single subcontractor contract based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getSubcontractor($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getSubcontractor: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\SubcontractorContract**](../Model/SubcontractorContract.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubcontractorContractHistoryEntries**
> \Swagger\Client\Model\SubcontractorContractHistory[] getSubcontractorContractHistoryEntries($id)

Returns a list of subcontractor contract history entries associated with the given ID.

Returns a list of subcontractor contract history entries.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Subcontractor contract ID

try {
    $result = $apiInstance->getSubcontractorContractHistoryEntries($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getSubcontractorContractHistoryEntries: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Subcontractor contract ID |

### Return type

[**\Swagger\Client\Model\SubcontractorContractHistory[]**](../Model/SubcontractorContractHistory.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubcontractorStatuses**
> object[] getSubcontractorStatuses()

Returns available statuses for a subcontractor contract.

Returns available statuses for a subcontractor contract.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getSubcontractorStatuses();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->getSubcontractorStatuses: ', $e->getMessage(), PHP_EOL;
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

# **listContractOrderLines**
> \Swagger\Client\Model\ContractOrderLineList listContractOrderLines($q)

Returns all contract order lines for the current organization. Use HQL to filter for specific items.

Returns all contract order lines for the current organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listContractOrderLines($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->listContractOrderLines: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\ContractOrderLineList**](../Model/ContractOrderLineList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPurchaseOrderContractTerms**
> \Swagger\Client\Model\PurchaseOrderContractTermList listPurchaseOrderContractTerms($q)

Returns a list of purchase order contract terms.

Returns a list of purchase order contract terms.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listPurchaseOrderContractTerms($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->listPurchaseOrderContractTerms: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\PurchaseOrderContractTermList**](../Model/PurchaseOrderContractTermList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listPurchaseOrderContracts**
> \Swagger\Client\Model\PurchaseOrderContractList listPurchaseOrderContracts($q)

Returns a list of purchase order contracts.

Returns a list of purchase order contracts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listPurchaseOrderContracts($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->listPurchaseOrderContracts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\PurchaseOrderContractList**](../Model/PurchaseOrderContractList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listSubcontractorContractTerms**
> \Swagger\Client\Model\SubcontractorContractTermList listSubcontractorContractTerms($q)

Returns a list of subcontractor contract terms.

Returns a list of subcontractor contract terms.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listSubcontractorContractTerms($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->listSubcontractorContractTerms: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\SubcontractorContractTermList**](../Model/SubcontractorContractTermList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listSubcontractorContracts**
> \Swagger\Client\Model\SubcontractorContractList listSubcontractorContracts($q)

Returns a list of subcontractor contracts.

Returns a list of subcontractor contracts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listSubcontractorContracts($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->listSubcontractorContracts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\SubcontractorContractList**](../Model/SubcontractorContractList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postContractOrderLine**
> \Swagger\Client\Model\ContractOrderLine postContractOrderLine($project, $body)

Create or update the contract order line.

Create or update a contract order line with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID
$body = new \Swagger\Client\Model\ContractOrderLine(); // \Swagger\Client\Model\ContractOrderLine | 

try {
    $result = $apiInstance->postContractOrderLine($project, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->postContractOrderLine: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |
 **body** | [**\Swagger\Client\Model\ContractOrderLine**](../Model/ContractOrderLine.md)|  |

### Return type

[**\Swagger\Client\Model\ContractOrderLine**](../Model/ContractOrderLine.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postPurchaseOrder**
> \Swagger\Client\Model\PurchaseOrderContract postPurchaseOrder($body)

Create or update a purchase order contract with the schema.

Create or update a purchase order contract with the corresponding schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PurchaseOrderContract(); // \Swagger\Client\Model\PurchaseOrderContract | 

try {
    $result = $apiInstance->postPurchaseOrder($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->postPurchaseOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PurchaseOrderContract**](../Model/PurchaseOrderContract.md)|  |

### Return type

[**\Swagger\Client\Model\PurchaseOrderContract**](../Model/PurchaseOrderContract.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postPurchaseOrderContractTerm**
> \Swagger\Client\Model\ContractTerm postPurchaseOrderContractTerm($body)

Create or update the purchase order contract term.

Create or update a purchase order contract term with the corresponding schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ContractTerm(); // \Swagger\Client\Model\ContractTerm | 

try {
    $result = $apiInstance->postPurchaseOrderContractTerm($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->postPurchaseOrderContractTerm: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)|  |

### Return type

[**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postSubcontractor**
> \Swagger\Client\Model\SubcontractorContract postSubcontractor($body)

Create or update a subcontractor contract with the schema.

Create or update a subcontractor contract with the corresponding schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SubcontractorContract(); // \Swagger\Client\Model\SubcontractorContract | 

try {
    $result = $apiInstance->postSubcontractor($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->postSubcontractor: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SubcontractorContract**](../Model/SubcontractorContract.md)|  |

### Return type

[**\Swagger\Client\Model\SubcontractorContract**](../Model/SubcontractorContract.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postSubcontractorContractTerm**
> \Swagger\Client\Model\ContractTerm postSubcontractorContractTerm($body)

Create or update the subcontractor contract term.

Create or update a subcontractor contract term with the corresponding schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ContractTerm(); // \Swagger\Client\Model\ContractTerm | 

try {
    $result = $apiInstance->postSubcontractorContractTerm($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->postSubcontractorContractTerm: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)|  |

### Return type

[**\Swagger\Client\Model\ContractTerm**](../Model/ContractTerm.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updatePurchaseOrderStatus**
> updatePurchaseOrderStatus($id, $status)

Update the purchase order contract with the given status.

Update the purchase order contract with the given status.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 
$status = 56; // int | 

try {
    $apiInstance->updatePurchaseOrderStatus($id, $status);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->updatePurchaseOrderStatus: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **status** | **int**|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateSubcontractorStatus**
> updateSubcontractorStatus($id, $status)

Update the subcontractor contract with the given status.

Update the subcontractor contract with the given status.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContractApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 
$status = 56; // int | 

try {
    $apiInstance->updateSubcontractorStatus($id, $status);
} catch (Exception $e) {
    echo 'Exception when calling ContractApi->updateSubcontractorStatus: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **status** | **int**|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

