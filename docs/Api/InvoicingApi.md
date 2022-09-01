# Swagger\Client\InvoicingApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteInvoice**](InvoicingApi.md#deleteInvoice) | **DELETE** /invoice/{invoice} | Delete the given invoice.
[**getCollectiveInvoicePdf**](InvoicingApi.md#getCollectiveInvoicePdf) | **GET** /invoice/{invoice}/collective-pdf | Returns the PDF of an invoice by the given ID.
[**getInvoice**](InvoicingApi.md#getInvoice) | **GET** /invoice/{invoice} | Returns the document of an existing invoice.
[**getInvoiceCompanyInfo**](InvoicingApi.md#getInvoiceCompanyInfo) | **GET** /invoicing-project/{project}/company-info | Returns the company information based on the given project.
[**getInvoiceEquipmentListPdf**](InvoicingApi.md#getInvoiceEquipmentListPdf) | **GET** /invoice/{invoice}/pdf/equipment-list | Returns the equipment list PDF of an invoice by the given ID.
[**getInvoiceGarbageListPdf**](InvoicingApi.md#getInvoiceGarbageListPdf) | **GET** /invoice/{invoice}/pdf/garbage-list | Returns the waste list PDF of an invoice by the given ID.
[**getInvoiceMailStatuses**](InvoicingApi.md#getInvoiceMailStatuses) | **GET** /invoice/mail-statuses | Returns available statuses for an invoice mail.
[**getInvoiceMaterialListPdf**](InvoicingApi.md#getInvoiceMaterialListPdf) | **GET** /invoice/{invoice}/pdf/material-list | Returns the material list of an invoice by the given ID.
[**getInvoicePdf**](InvoicingApi.md#getInvoicePdf) | **GET** /invoice/{invoice}/pdf | Returns the PDF of an invoice by the given ID.
[**listInvoices**](InvoicingApi.md#listInvoices) | **GET** /list/invoices | Returns a list of invoices associated with the organization.
[**makeAttachments**](InvoicingApi.md#makeAttachments) | **POST** /invoice/{invoice}/make-attachments | Generate the given attachments for the given invoice.
[**newInvoice**](InvoicingApi.md#newInvoice) | **GET** /invoice/new | Returns the document of a new invoice.
[**newInvoiceForProject**](InvoicingApi.md#newInvoiceForProject) | **GET** /project/{project}/invoice/new | Returns the document of a new invoice.
[**updateInvoice**](InvoicingApi.md#updateInvoice) | **POST** /invoice | Creates or updates an invoice based on the given document.


# **deleteInvoice**
> deleteInvoice($invoice)

Delete the given invoice.

Delete the given invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $apiInstance->deleteInvoice($invoice);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->deleteInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCollectiveInvoicePdf**
> string getCollectiveInvoicePdf($invoice)

Returns the PDF of an invoice by the given ID.

Returns the PDF of an collective invoice by the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $result = $apiInstance->getCollectiveInvoicePdf($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getCollectiveInvoicePdf: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoice**
> \Swagger\Client\Model\InvoiceDocument getInvoice($invoice)

Returns the document of an existing invoice.

Returns the document of a new invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $result = $apiInstance->getInvoice($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

[**\Swagger\Client\Model\InvoiceDocument**](../Model/InvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoiceCompanyInfo**
> \Swagger\Client\Model\InvoiceOrganization getInvoiceCompanyInfo($project)

Returns the company information based on the given project.

Returns the company information based on the given project.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID

try {
    $result = $apiInstance->getInvoiceCompanyInfo($project);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoiceCompanyInfo: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |

### Return type

[**\Swagger\Client\Model\InvoiceOrganization**](../Model/InvoiceOrganization.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoiceEquipmentListPdf**
> string getInvoiceEquipmentListPdf($invoice)

Returns the equipment list PDF of an invoice by the given ID.

Returns the equipment list PDF of a invoice by the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Equipment ID

try {
    $result = $apiInstance->getInvoiceEquipmentListPdf($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoiceEquipmentListPdf: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Equipment ID |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoiceGarbageListPdf**
> string getInvoiceGarbageListPdf($invoice)

Returns the waste list PDF of an invoice by the given ID.

Returns the waste list PDF of a invoice by the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $result = $apiInstance->getInvoiceGarbageListPdf($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoiceGarbageListPdf: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoiceMailStatuses**
> string[] getInvoiceMailStatuses()

Returns available statuses for an invoice mail.

Returns available statuses for an invoice mail.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getInvoiceMailStatuses();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoiceMailStatuses: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

**string[]**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoiceMaterialListPdf**
> string getInvoiceMaterialListPdf($invoice)

Returns the material list of an invoice by the given ID.

Returns the material list of a invoice by the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $result = $apiInstance->getInvoiceMaterialListPdf($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoiceMaterialListPdf: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoicePdf**
> string getInvoicePdf($invoice)

Returns the PDF of an invoice by the given ID.

Returns the PDF of an invoice by the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | Invoice ID

try {
    $result = $apiInstance->getInvoicePdf($invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->getInvoicePdf: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| Invoice ID |

### Return type

**string**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listInvoices**
> \Swagger\Client\Model\InvoiceList listInvoices($q)

Returns a list of invoices associated with the organization.

Returns a list of invoices associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listInvoices($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->listInvoices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\InvoiceList**](../Model/InvoiceList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **makeAttachments**
> \Swagger\Client\Model\InvoiceAttachment[] makeAttachments($invoice, $generate_attachment)

Generate the given attachments for the given invoice.

Generate the given attachments for the given invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice = 56; // int | The invoice for which to generate the attachments.
$generate_attachment = new \Swagger\Client\Model\GenerateAttachment(); // \Swagger\Client\Model\GenerateAttachment | Which attachments to generate and attach to the given invoice.

try {
    $result = $apiInstance->makeAttachments($invoice, $generate_attachment);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->makeAttachments: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice** | **int**| The invoice for which to generate the attachments. |
 **generate_attachment** | [**\Swagger\Client\Model\GenerateAttachment**](../Model/GenerateAttachment.md)| Which attachments to generate and attach to the given invoice. |

### Return type

[**\Swagger\Client\Model\InvoiceAttachment[]**](../Model/InvoiceAttachment.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **newInvoice**
> \Swagger\Client\Model\InvoiceDocument newInvoice()

Returns the document of a new invoice.

Returns the document of a new invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->newInvoice();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->newInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InvoiceDocument**](../Model/InvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **newInvoiceForProject**
> \Swagger\Client\Model\InvoiceDocument newInvoiceForProject($project)

Returns the document of a new invoice.

Returns the document of a new invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID

try {
    $result = $apiInstance->newInvoiceForProject($project);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->newInvoiceForProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |

### Return type

[**\Swagger\Client\Model\InvoiceDocument**](../Model/InvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateInvoice**
> \Swagger\Client\Model\InvoiceDocument updateInvoice($invoice_document)

Creates or updates an invoice based on the given document.

Returns the document of a new invoice.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\InvoicingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice_document = new \Swagger\Client\Model\InvoiceDocument(); // \Swagger\Client\Model\InvoiceDocument | The invoice document to save.

try {
    $result = $apiInstance->updateInvoice($invoice_document);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicingApi->updateInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_document** | [**\Swagger\Client\Model\InvoiceDocument**](../Model/InvoiceDocument.md)| The invoice document to save. |

### Return type

[**\Swagger\Client\Model\InvoiceDocument**](../Model/InvoiceDocument.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

