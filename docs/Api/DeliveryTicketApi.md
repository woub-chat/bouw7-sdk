# Swagger\Client\DeliveryTicketApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteDeliveryTicket**](DeliveryTicketApi.md#deleteDeliveryTicket) | **DELETE** /project/delivery-ticket | Delete the given delivery ticket.
[**getDeliveryTicket**](DeliveryTicketApi.md#getDeliveryTicket) | **GET** /project/delivery-ticket/{id} | Returns a single delivery ticket based on the given ID.
[**getPurchaseTypes**](DeliveryTicketApi.md#getPurchaseTypes) | **GET** /delivery-ticket/purchase-types | Returns available purchase types for a delivery ticket.
[**listDeliveryTickets**](DeliveryTicketApi.md#listDeliveryTickets) | **GET** /list/delivery-tickets | Returns a list of delivery tickets associated with your organization.
[**postDeliveryTicket**](DeliveryTicketApi.md#postDeliveryTicket) | **POST** /project/delivery-ticket | Create or update the delivery ticket.


# **deleteDeliveryTicket**
> deleteDeliveryTicket($body)

Delete the given delivery ticket.

Delete the given delivery ticket.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DeliveryTicketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DeliveryTicket(); // \Swagger\Client\Model\DeliveryTicket | 

try {
    $apiInstance->deleteDeliveryTicket($body);
} catch (Exception $e) {
    echo 'Exception when calling DeliveryTicketApi->deleteDeliveryTicket: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DeliveryTicket**](../Model/DeliveryTicket.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDeliveryTicket**
> \Swagger\Client\Model\DeliveryTicket getDeliveryTicket($id)

Returns a single delivery ticket based on the given ID.

Returns a single delivery ticket based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DeliveryTicketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getDeliveryTicket($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DeliveryTicketApi->getDeliveryTicket: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\DeliveryTicket**](../Model/DeliveryTicket.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPurchaseTypes**
> object[] getPurchaseTypes()

Returns available purchase types for a delivery ticket.

Returns available purchase types for a delivery ticket.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DeliveryTicketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getPurchaseTypes();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DeliveryTicketApi->getPurchaseTypes: ', $e->getMessage(), PHP_EOL;
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

# **listDeliveryTickets**
> \Swagger\Client\Model\DeliveryTicketList listDeliveryTickets($q)

Returns a list of delivery tickets associated with your organization.

Returns a list of delivery tickets associated your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DeliveryTicketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string.

try {
    $result = $apiInstance->listDeliveryTickets($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DeliveryTicketApi->listDeliveryTickets: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string. | [optional]

### Return type

[**\Swagger\Client\Model\DeliveryTicketList**](../Model/DeliveryTicketList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postDeliveryTicket**
> \Swagger\Client\Model\DeliveryTicket postDeliveryTicket($body)

Create or update the delivery ticket.

Create or update a delivery ticket with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\DeliveryTicketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\DeliveryTicket(); // \Swagger\Client\Model\DeliveryTicket | 

try {
    $result = $apiInstance->postDeliveryTicket($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DeliveryTicketApi->postDeliveryTicket: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\DeliveryTicket**](../Model/DeliveryTicket.md)|  |

### Return type

[**\Swagger\Client\Model\DeliveryTicket**](../Model/DeliveryTicket.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

