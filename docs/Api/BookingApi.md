# Swagger\Client\BookingApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findBookingLines**](BookingApi.md#findBookingLines) | **GET** /project/{project}/booking-lines | Returns all available booking items based on its criteria.


# **findBookingLines**
> \Swagger\Client\Model\BookingList findBookingLines($project, $start_date, $end_date, $type, $invoice_cost_status_ids, $project_security_link_ids, $find_for_checkout_document)

Returns all available booking items based on its criteria.

Returns all available booking items based on its criteria.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\BookingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$project = 56; // int | Project ID
$start_date = "start_date_example"; // string | Start date
$end_date = "end_date_example"; // string | End date
$type = 56; // int | Type bit mask
$invoice_cost_status_ids = array(56); // int[] | Include booking objects where invoiceCostStatusId is in this list.
$project_security_link_ids = array(56); // int[] | The project security link IDs to filter booking items by. Excludes items with no relation by default.
$find_for_checkout_document = 56; // int | Whether the booking lines should be retrieved for a checkout document. Available values: 0, 1.

try {
    $result = $apiInstance->findBookingLines($project, $start_date, $end_date, $type, $invoice_cost_status_ids, $project_security_link_ids, $find_for_checkout_document);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BookingApi->findBookingLines: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | **int**| Project ID |
 **start_date** | **string**| Start date | [optional]
 **end_date** | **string**| End date | [optional]
 **type** | **int**| Type bit mask | [optional]
 **invoice_cost_status_ids** | [**int[]**](../Model/int.md)| Include booking objects where invoiceCostStatusId is in this list. | [optional]
 **project_security_link_ids** | [**int[]**](../Model/int.md)| The project security link IDs to filter booking items by. Excludes items with no relation by default. | [optional]
 **find_for_checkout_document** | **int**| Whether the booking lines should be retrieved for a checkout document. Available values: 0, 1. | [optional]

### Return type

[**\Swagger\Client\Model\BookingList**](../Model/BookingList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

