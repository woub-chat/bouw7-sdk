# Swagger\Client\AuditLogApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getPurchaseInvoiceAuditLogs**](AuditLogApi.md#getPurchaseInvoiceAuditLogs) | **GET** /purchase-invoice/{purchaseInvoice}/audit-logs | Get all purchase invoice audit logs.
[**getQuotationAuditLogs**](AuditLogApi.md#getQuotationAuditLogs) | **GET** /quotation/{quotation}/audit-logs | Get all Quotation audit logs.


# **getPurchaseInvoiceAuditLogs**
> \Swagger\Client\Model\AuditLog[] getPurchaseInvoiceAuditLogs($purchase_invoice)

Get all purchase invoice audit logs.

List all purchase invoice audit logs for the given purchase invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AuditLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$purchase_invoice = 56; // int | Purchase invoice ID

try {
    $result = $apiInstance->getPurchaseInvoiceAuditLogs($purchase_invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuditLogApi->getPurchaseInvoiceAuditLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_invoice** | **int**| Purchase invoice ID |

### Return type

[**\Swagger\Client\Model\AuditLog[]**](../Model/AuditLog.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getQuotationAuditLogs**
> \Swagger\Client\Model\AuditLog[] getQuotationAuditLogs($quotation)

Get all Quotation audit logs.

List all Quotation audit logs for the given Quotation.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AuditLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quotation = 56; // int | Quotation ID

try {
    $result = $apiInstance->getQuotationAuditLogs($quotation);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuditLogApi->getQuotationAuditLogs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotation** | **int**| Quotation ID |

### Return type

[**\Swagger\Client\Model\AuditLog[]**](../Model/AuditLog.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

