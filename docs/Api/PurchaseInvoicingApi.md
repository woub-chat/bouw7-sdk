# Swagger\Client\PurchaseInvoicingApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deletePurchaseInvoice**](PurchaseInvoicingApi.md#deletePurchaseInvoice) | **DELETE** /purchase-invoice | Delete the given purchase invoice.
[**getDefaultGeneralLedgerAccountCode**](PurchaseInvoicingApi.md#getDefaultGeneralLedgerAccountCode) | **POST** /purchase-invoicing/default-general-ledger-account | Returns the default general ledger account based on the given contact id / branch id.
[**getPurchaseInvoice**](PurchaseInvoicingApi.md#getPurchaseInvoice) | **GET** /purchase-invoicing/purchase-invoice/{id} | Returns a single purchase invoice based on the given ID.
[**getPurchaseInvoiceStatuses**](PurchaseInvoicingApi.md#getPurchaseInvoiceStatuses) | **GET** /purchase-invoicing/statuses | Returns available statuses for an purchase invoice.
[**listPurchaseInvoices**](PurchaseInvoicingApi.md#listPurchaseInvoices) | **GET** /list/purchase-invoices | Returns a list of purchase invoices belonging to the organization.
[**postPurchaseInvoice**](PurchaseInvoicingApi.md#postPurchaseInvoice) | **POST** /purchase-invoice | Create or update purchase invoice.
[**updatePurchaseInvoiceStatus**](PurchaseInvoicingApi.md#updatePurchaseInvoiceStatus) | **PUT** /purchase-invoice/{id}/update-status/{status} | Update the purchase invoice with the given status.


# **deletePurchaseInvoice**
> deletePurchaseInvoice($body)

Delete the given purchase invoice.

Delete the given purchase invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedPurchaseInvoice(); // \Swagger\Client\Model\CondensedPurchaseInvoice | 

try {
    $apiInstance->deletePurchaseInvoice($body);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->deletePurchaseInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedPurchaseInvoice**](../Model/CondensedPurchaseInvoice.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDefaultGeneralLedgerAccountCode**
> string getDefaultGeneralLedgerAccountCode($body)

Returns the default general ledger account based on the given contact id / branch id.

Returns the default general ledger account based on the given contact id / branch id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DefaultPurchaseInvoiceSettingsFilter(); // \Swagger\Client\Model\DefaultPurchaseInvoiceSettingsFilter | 

try {
    $result = $apiInstance->getDefaultGeneralLedgerAccountCode($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->getDefaultGeneralLedgerAccountCode: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DefaultPurchaseInvoiceSettingsFilter**](../Model/DefaultPurchaseInvoiceSettingsFilter.md)|  |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseInvoice**
> \Swagger\Client\Model\PurchaseInvoiceDocument getPurchaseInvoice($id)

Returns a single purchase invoice based on the given ID.

Returns a single purchase invoice based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getPurchaseInvoice($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->getPurchaseInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\PurchaseInvoiceDocument**](../Model/PurchaseInvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseInvoiceStatuses**
> object[] getPurchaseInvoiceStatuses()

Returns available statuses for an purchase invoice.

Returns available statuses for an purchase invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getPurchaseInvoiceStatuses();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->getPurchaseInvoiceStatuses: ', $e->getMessage(), PHP_EOL;
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

# **listPurchaseInvoices**
> \Swagger\Client\Model\PurchaseInvoiceList listPurchaseInvoices($q)

Returns a list of purchase invoices belonging to the organization.

Returns a list of pruchase invoices belonging to the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listPurchaseInvoices($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->listPurchaseInvoices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\PurchaseInvoiceList**](../Model/PurchaseInvoiceList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postPurchaseInvoice**
> \Swagger\Client\Model\PurchaseInvoiceDocument postPurchaseInvoice($body)

Create or update purchase invoice.

Create or update a purchase invoice with the corresponding schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\PurchaseInvoiceDocument(); // \Swagger\Client\Model\PurchaseInvoiceDocument | 

try {
    $result = $apiInstance->postPurchaseInvoice($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->postPurchaseInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\PurchaseInvoiceDocument**](../Model/PurchaseInvoiceDocument.md)|  |

### Return type

[**\Swagger\Client\Model\PurchaseInvoiceDocument**](../Model/PurchaseInvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updatePurchaseInvoiceStatus**
> updatePurchaseInvoiceStatus($id, $status)

Update the purchase invoice with the given status.

Update the purchase invoice with the given status.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\PurchaseInvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 
$status = 56; // int | 

try {
    $apiInstance->updatePurchaseInvoiceStatus($id, $status);
} catch (Exception $e) {
    echo 'Exception when calling PurchaseInvoicingApi->updatePurchaseInvoiceStatus: ', $e->getMessage(), PHP_EOL;
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

