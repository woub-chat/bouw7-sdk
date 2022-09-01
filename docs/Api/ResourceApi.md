# Swagger\Client\ResourceApi

All URIs are relative to *https://heimdall.bouw7.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteEquipment**](ResourceApi.md#deleteEquipment) | **DELETE** /equipment | Deletes an equipment item associated with the given id.
[**deleteEquipmentBooking**](ResourceApi.md#deleteEquipmentBooking) | **DELETE** /equipment-booking | Deletes an equipment booking associated with the given id.
[**deleteEquipmentGroup**](ResourceApi.md#deleteEquipmentGroup) | **DELETE** /equipment-group | Deletes an equipment group associated with the given id.
[**deleteEquipmentUnit**](ResourceApi.md#deleteEquipmentUnit) | **DELETE** /equipment-unit/{id} | Deletes an equipment unit associated with the given ID.
[**deleteMaterial**](ResourceApi.md#deleteMaterial) | **DELETE** /material/{material} | Deletes a material item associated with the given ID.
[**deleteMaterialBooking**](ResourceApi.md#deleteMaterialBooking) | **DELETE** /material-booking | Deletes a material booking associated with the given ID.
[**deleteMaterialPerUnit**](ResourceApi.md#deleteMaterialPerUnit) | **DELETE** /material-per-unit | Deletes the given material per unit.
[**deleteMaterialUnit**](ResourceApi.md#deleteMaterialUnit) | **DELETE** /material-unit/{id} | Deletes a material unit associated with the given ID.
[**deleteResource**](ResourceApi.md#deleteResource) | **DELETE** /resource | Deletes a resource associated with the given id.
[**deleteResourceBooking**](ResourceApi.md#deleteResourceBooking) | **DELETE** /resource-booking | Deletes a resource booking associated with the given id.
[**deleteResourceGroup**](ResourceApi.md#deleteResourceGroup) | **DELETE** /resource-group | Deletes a resource group associated with the given id.
[**deleteResourceUnit**](ResourceApi.md#deleteResourceUnit) | **DELETE** /resource-unit | Deletes a resource unit associated with the given id.
[**deleteWaste**](ResourceApi.md#deleteWaste) | **DELETE** /waste/{id} | Deletes a waste item associated with the given id.
[**deleteWasteBooking**](ResourceApi.md#deleteWasteBooking) | **DELETE** /waste-booking | Deletes a waste booking associated with the given ID.
[**deleteWastePerUnit**](ResourceApi.md#deleteWastePerUnit) | **DELETE** /waste-per-unit | Deletes the given waste per unit.
[**deleteWasteUnit**](ResourceApi.md#deleteWasteUnit) | **DELETE** /waste-unit/{wasteUnit} | Deletes a waste unit associated with the given ID.
[**getEquipment**](ResourceApi.md#getEquipment) | **GET** /equipment/{equipment} | Returns a single equipment item based on the given ID.
[**getEquipmentBooking**](ResourceApi.md#getEquipmentBooking) | **GET** /equipment-booking/{id} | Returns an equipment booking associated with the given id.
[**getEquipmentGroup**](ResourceApi.md#getEquipmentGroup) | **GET** /equipment-group/{id} | Returns an equipment group associated with the given id.
[**getEquipmentGroups**](ResourceApi.md#getEquipmentGroups) | **GET** /equipment-groups | Returns a list of equipment groups associated with the organization.
[**getEquipmentUnit**](ResourceApi.md#getEquipmentUnit) | **GET** /equipment-unit/{equipmentUnit} | Returns a single equipment unit based on the given ID.
[**getMaterial**](ResourceApi.md#getMaterial) | **GET** /material/{id} | Returns a single material based on the given ID.
[**getMaterialPerUnit**](ResourceApi.md#getMaterialPerUnit) | **GET** /material-per-unit/{id} | Returns a single material per unit based on the given ID.
[**getMaterialUnit**](ResourceApi.md#getMaterialUnit) | **GET** /material-unit/{materialUnit} | Returns a single material unit based on the given ID.
[**getResource**](ResourceApi.md#getResource) | **GET** /resource/{type}/{id} | Returns a resource associated with the given id.
[**getResourceBooking**](ResourceApi.md#getResourceBooking) | **GET** /resource-booking/{type}/{id} | Returns a resource booking associated with the given id.
[**getResourceBookings**](ResourceApi.md#getResourceBookings) | **GET** /resource-bookings/{type} | Returns a set of resource bookings by an organization, optionally filtered by project.
[**getResourceGroup**](ResourceApi.md#getResourceGroup) | **GET** /resource-group/{type}/{id} | Returns an resource group associated with the given id.
[**getResourceUnit**](ResourceApi.md#getResourceUnit) | **GET** /resource-unit/{type}/{id} | Returns a resource unit associated with the given id.
[**getResourceUnits**](ResourceApi.md#getResourceUnits) | **GET** /resource-units/{type} | Returns a set of resource units associated with the organization.
[**getResources**](ResourceApi.md#getResources) | **GET** /resources/{type} | Returns a set of resources associated with the organization.
[**getWaste**](ResourceApi.md#getWaste) | **GET** /waste/{waste} | Returns a single waste item based on the given ID.
[**getWasteBooking**](ResourceApi.md#getWasteBooking) | **GET** /waste-booking/{wasteBooking} | Returns a waste booking associated with the given ID.
[**getWastePerUnit**](ResourceApi.md#getWastePerUnit) | **GET** /waste-per-unit/{id} | Returns a single waste per unit based on the given ID.
[**getWasteUnit**](ResourceApi.md#getWasteUnit) | **GET** /waste-unit/{id} | Returns a single waste unit based on the given ID.
[**importMaterialPerUnits**](ResourceApi.md#importMaterialPerUnits) | **POST** /import/material-per-unit | Creates material records based on the given material per unit import list if the data is unique.
[**importWastePerUnits**](ResourceApi.md#importWastePerUnits) | **POST** /import/waste-per-unit | Creates waste records based on the given waste per unit import list if the data is unique.
[**listEquipment**](ResourceApi.md#listEquipment) | **GET** /list/equipment | Returns a list of equipment items owned by the organization.
[**listEquipmentBookings**](ResourceApi.md#listEquipmentBookings) | **GET** /list/booking/equipment | Returns a list of equipment bookings made by the organization.
[**listEquipmentGroups**](ResourceApi.md#listEquipmentGroups) | **GET** /list/equipment-groups | Returns a list of equipment groups owned by your organization.
[**listEquipmentPerUnit**](ResourceApi.md#listEquipmentPerUnit) | **GET** /list/equipment-per-unit | Returns a bookable list of units associated with a piece of equipment.
[**listEquipmentUnits**](ResourceApi.md#listEquipmentUnits) | **GET** /list/equipment-units | Returns a list of equipment units owned by your organization.
[**listGarbage**](ResourceApi.md#listGarbage) | **GET** /list/garbage | Returns a list of waste owned by the organization.
[**listGarbageBookings**](ResourceApi.md#listGarbageBookings) | **GET** /list/booking/garbage | Returns a list of waste bookings made by the organization.
[**listGarbagePerUnit**](ResourceApi.md#listGarbagePerUnit) | **GET** /list/garbage-per-unit | Returns a bookable list of units associated with waste.
[**listMaterialBookings**](ResourceApi.md#listMaterialBookings) | **GET** /list/booking/material | Returns a list of material bookings made by the organization.
[**listMaterialUnits**](ResourceApi.md#listMaterialUnits) | **GET** /list/material-units | Returns a list of material units owned by your organization.
[**listMaterials**](ResourceApi.md#listMaterials) | **GET** /list/materials | Returns a list of materials owned by your organization.
[**listMaterialsPerUnit**](ResourceApi.md#listMaterialsPerUnit) | **GET** /list/materials-per-unit | Returns a bookable list of units associated with materials.
[**listWaste**](ResourceApi.md#listWaste) | **GET** /list/waste | Returns a list of waste items owned by your organization.
[**listWastePerUnit**](ResourceApi.md#listWastePerUnit) | **GET** /list/waste-per-unit | Returns a bookable list of units associated with waste.
[**listWasteUnits**](ResourceApi.md#listWasteUnits) | **GET** /list/waste-units | Returns a list of waste units owned by your organization.
[**postEquipment**](ResourceApi.md#postEquipment) | **POST** /equipment | Create or update an equipment item.
[**postEquipmentBooking**](ResourceApi.md#postEquipmentBooking) | **POST** /equipment-booking | Create or update the equipment booking.
[**postEquipmentGroup**](ResourceApi.md#postEquipmentGroup) | **POST** /equipment-group | Creates or updates an equipment group for the currently authenticated user.
[**postEquipmentUnit**](ResourceApi.md#postEquipmentUnit) | **POST** /equipment-unit | Create or update the equipment unit.
[**postMaterial**](ResourceApi.md#postMaterial) | **POST** /material | Create or update the material.
[**postMaterialPerUnit**](ResourceApi.md#postMaterialPerUnit) | **POST** /material-per-unit | Create or update the material per unit.
[**postMaterialUnit**](ResourceApi.md#postMaterialUnit) | **POST** /material-unit | Create or update the material unit.
[**postResource**](ResourceApi.md#postResource) | **POST** /resource | Creates or updates a resource for the currently authenticated user.
[**postResourceBooking**](ResourceApi.md#postResourceBooking) | **POST** /resource-booking | Creates or updates a resource booking for the currently authenticated user.
[**postResourceGroup**](ResourceApi.md#postResourceGroup) | **POST** /resource-group | Creates or updates a resource group for the currently authenticated user.
[**postResourceUnit**](ResourceApi.md#postResourceUnit) | **POST** /resource-unit | Creates or updates a resource unit for the currently authenticated user.
[**postWaste**](ResourceApi.md#postWaste) | **POST** /waste | Create or update a waste item.
[**postWasteUnit**](ResourceApi.md#postWasteUnit) | **POST** /waste-unit | Create or update the waste unit.


# **deleteEquipment**
> deleteEquipment($body)

Deletes an equipment item associated with the given id.

Delete the given equipment item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedEquipment(); // \Swagger\Client\Model\CondensedEquipment | 

try {
    $apiInstance->deleteEquipment($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteEquipment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedEquipment**](../Model/CondensedEquipment.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteEquipmentBooking**
> deleteEquipmentBooking($body)

Deletes an equipment booking associated with the given id.

Deletes an equipment booking associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedEquipmentBooking(); // \Swagger\Client\Model\CondensedEquipmentBooking | 

try {
    $apiInstance->deleteEquipmentBooking($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteEquipmentBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedEquipmentBooking**](../Model/CondensedEquipmentBooking.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteEquipmentGroup**
> deleteEquipmentGroup($body)

Deletes an equipment group associated with the given id.

Deletes an equipment group associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\EquipmentGroup(); // \Swagger\Client\Model\EquipmentGroup | 

try {
    $apiInstance->deleteEquipmentGroup($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteEquipmentGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\EquipmentGroup**](../Model/EquipmentGroup.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteEquipmentUnit**
> deleteEquipmentUnit($id, $equipment_unit_replacement_id)

Deletes an equipment unit associated with the given ID.

Delete the given equipment unit.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | The ID of the equipment unit that will be deleted.
$equipment_unit_replacement_id = 56; // int | The ID of the equipment unit that will be used to replace references of the deleted equipment unit on associated equipment per units.

try {
    $apiInstance->deleteEquipmentUnit($id, $equipment_unit_replacement_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteEquipmentUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the equipment unit that will be deleted. |
 **equipment_unit_replacement_id** | **int**| The ID of the equipment unit that will be used to replace references of the deleted equipment unit on associated equipment per units. | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteMaterial**
> deleteMaterial($material, $material_replacement_id)

Deletes a material item associated with the given ID.

Delete the given material.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$material = 56; // int | The ID of the material that will be deleted.
$material_replacement_id = 56; // int | The ID of the material that will be used to replace references of the deleted material on associated material per units.

try {
    $apiInstance->deleteMaterial($material, $material_replacement_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **material** | **int**| The ID of the material that will be deleted. |
 **material_replacement_id** | **int**| The ID of the material that will be used to replace references of the deleted material on associated material per units. | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteMaterialBooking**
> deleteMaterialBooking($body)

Deletes a material booking associated with the given ID.

Delete the given material booking.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedMaterialBooking(); // \Swagger\Client\Model\CondensedMaterialBooking | 

try {
    $apiInstance->deleteMaterialBooking($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteMaterialBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedMaterialBooking**](../Model/CondensedMaterialBooking.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteMaterialPerUnit**
> deleteMaterialPerUnit($body)

Deletes the given material per unit.

Delete the given material per unit.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedMaterialPerUnit(); // \Swagger\Client\Model\CondensedMaterialPerUnit | 

try {
    $apiInstance->deleteMaterialPerUnit($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteMaterialPerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedMaterialPerUnit**](../Model/CondensedMaterialPerUnit.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteMaterialUnit**
> deleteMaterialUnit($id, $material_unit_replacement_id)

Deletes a material unit associated with the given ID.

Delete the given material unit.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | The ID of the material unit that will be deleted.
$material_unit_replacement_id = 56; // int | The ID of the material unit that will be used to replace references of the deleted material unit on associated material per units.

try {
    $apiInstance->deleteMaterialUnit($id, $material_unit_replacement_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteMaterialUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the material unit that will be deleted. |
 **material_unit_replacement_id** | **int**| The ID of the material unit that will be used to replace references of the deleted material unit on associated material per units. | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteResource**
> deleteResource($body)

Deletes a resource associated with the given id.

Deletes a resource associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Resource(); // \Swagger\Client\Model\Resource | 

try {
    $apiInstance->deleteResource($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteResource: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Resource**](../Model/Resource.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteResourceBooking**
> deleteResourceBooking($body)

Deletes a resource booking associated with the given id.

Deletes a resource booking associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceBooking(); // \Swagger\Client\Model\ResourceBooking | 

try {
    $apiInstance->deleteResourceBooking($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteResourceBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceBooking**](../Model/ResourceBooking.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteResourceGroup**
> deleteResourceGroup($body)

Deletes a resource group associated with the given id.

Deletes a resource group associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceGroup(); // \Swagger\Client\Model\ResourceGroup | 

try {
    $apiInstance->deleteResourceGroup($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteResourceGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceGroup**](../Model/ResourceGroup.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteResourceUnit**
> deleteResourceUnit($body)

Deletes a resource unit associated with the given id.

Deletes a resource unit associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceUnit(); // \Swagger\Client\Model\ResourceUnit | 

try {
    $apiInstance->deleteResourceUnit($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteResourceUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceUnit**](../Model/ResourceUnit.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteWaste**
> deleteWaste($id, $waste_replacement_id)

Deletes a waste item associated with the given id.

Delete the given waste item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | The ID of the waste item that will be deleted.
$waste_replacement_id = 56; // int | The ID of the waste item that will be used to replace references of the deleted waste item on associated waste per units.

try {
    $apiInstance->deleteWaste($id, $waste_replacement_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteWaste: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the waste item that will be deleted. |
 **waste_replacement_id** | **int**| The ID of the waste item that will be used to replace references of the deleted waste item on associated waste per units. | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteWasteBooking**
> deleteWasteBooking($body)

Deletes a waste booking associated with the given ID.

Delete the given waste booking.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedWasteBooking(); // \Swagger\Client\Model\CondensedWasteBooking | 

try {
    $apiInstance->deleteWasteBooking($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteWasteBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedWasteBooking**](../Model/CondensedWasteBooking.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteWastePerUnit**
> deleteWastePerUnit($body)

Deletes the given waste per unit.

Delete the given waste per unit.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedWastePerUnit(); // \Swagger\Client\Model\CondensedWastePerUnit | 

try {
    $apiInstance->deleteWastePerUnit($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteWastePerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CondensedWastePerUnit**](../Model/CondensedWastePerUnit.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteWasteUnit**
> deleteWasteUnit($waste_unit, $waste_unit_replacement_id)

Deletes a waste unit associated with the given ID.

Delete the given waste unit.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$waste_unit = 56; // int | The ID of the waste unit that will be deleted.
$waste_unit_replacement_id = 56; // int | The ID of the waste unit that will be used to replace references of the deleted waste unit on associated waste per units.

try {
    $apiInstance->deleteWasteUnit($waste_unit, $waste_unit_replacement_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->deleteWasteUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **waste_unit** | **int**| The ID of the waste unit that will be deleted. |
 **waste_unit_replacement_id** | **int**| The ID of the waste unit that will be used to replace references of the deleted waste unit on associated waste per units. | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEquipment**
> \Swagger\Client\Model\Equipment getEquipment($equipment)

Returns a single equipment item based on the given ID.

Returns a single equipment item based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$equipment = 56; // int | 

try {
    $result = $apiInstance->getEquipment($equipment);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getEquipment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **equipment** | **int**|  |

### Return type

[**\Swagger\Client\Model\Equipment**](../Model/Equipment.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEquipmentBooking**
> \Swagger\Client\Model\EquipmentBooking getEquipmentBooking($id)

Returns an equipment booking associated with the given id.

Returns an equipment booking associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Equipment booking ID

try {
    $result = $apiInstance->getEquipmentBooking($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getEquipmentBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Equipment booking ID |

### Return type

[**\Swagger\Client\Model\EquipmentBooking**](../Model/EquipmentBooking.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEquipmentGroup**
> \Swagger\Client\Model\EquipmentGroup getEquipmentGroup($id)

Returns an equipment group associated with the given id.

Returns an equipment group associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | Equipment group ID

try {
    $result = $apiInstance->getEquipmentGroup($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getEquipmentGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Equipment group ID |

### Return type

[**\Swagger\Client\Model\EquipmentGroup**](../Model/EquipmentGroup.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEquipmentGroups**
> \Swagger\Client\Model\EquipmentGroup[] getEquipmentGroups()

Returns a list of equipment groups associated with the organization.

Returns a list of equipment groups associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getEquipmentGroups();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getEquipmentGroups: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\EquipmentGroup[]**](../Model/EquipmentGroup.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEquipmentUnit**
> \Swagger\Client\Model\EquipmentUnit getEquipmentUnit($equipment_unit)

Returns a single equipment unit based on the given ID.

Returns a single equipment unit based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$equipment_unit = 56; // int | 

try {
    $result = $apiInstance->getEquipmentUnit($equipment_unit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getEquipmentUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **equipment_unit** | **int**|  |

### Return type

[**\Swagger\Client\Model\EquipmentUnit**](../Model/EquipmentUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMaterial**
> \Swagger\Client\Model\Material getMaterial($id)

Returns a single material based on the given ID.

Returns a single material based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getMaterial($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\Material**](../Model/Material.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMaterialPerUnit**
> \Swagger\Client\Model\MaterialPerUnit getMaterialPerUnit($id)

Returns a single material per unit based on the given ID.

Returns a single material per unit based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getMaterialPerUnit($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getMaterialPerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\MaterialPerUnit**](../Model/MaterialPerUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMaterialUnit**
> \Swagger\Client\Model\MaterialUnit getMaterialUnit($material_unit)

Returns a single material unit based on the given ID.

Returns a single material unit based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$material_unit = 56; // int | 

try {
    $result = $apiInstance->getMaterialUnit($material_unit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getMaterialUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **material_unit** | **int**|  |

### Return type

[**\Swagger\Client\Model\MaterialUnit**](../Model/MaterialUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResource**
> \Swagger\Client\Model\Resource getResource($type, $id)

Returns a resource associated with the given id.

Returns a resource associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$id = 56; // int | Resource ID

try {
    $result = $apiInstance->getResource($type, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResource: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **id** | **int**| Resource ID |

### Return type

[**\Swagger\Client\Model\Resource**](../Model/Resource.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResourceBooking**
> \Swagger\Client\Model\ResourceBooking getResourceBooking($type, $id)

Returns a resource booking associated with the given id.

Returns a resource booking associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$id = 56; // int | Resource booking ID

try {
    $result = $apiInstance->getResourceBooking($type, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResourceBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **id** | **int**| Resource booking ID |

### Return type

[**\Swagger\Client\Model\ResourceBooking**](../Model/ResourceBooking.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResourceBookings**
> \Swagger\Client\Model\FilteredResourceBookingCollection getResourceBookings($type, $project_id, $q)

Returns a set of resource bookings by an organization, optionally filtered by project.

Returns a set of resource bookings by an organization, optionally filtered by project.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$project_id = 56; // int | The id of the project
$q = "q_example"; // string | Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language)

try {
    $result = $apiInstance->getResourceBookings($type, $project_id, $q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResourceBookings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **project_id** | **int**| The id of the project | [optional]
 **q** | **string**| Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) | [optional]

### Return type

[**\Swagger\Client\Model\FilteredResourceBookingCollection**](../Model/FilteredResourceBookingCollection.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResourceGroup**
> \Swagger\Client\Model\ResourceGroup getResourceGroup($type, $id)

Returns an resource group associated with the given id.

Returns a resource grgit oup associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$id = 56; // int | Resource group ID

try {
    $result = $apiInstance->getResourceGroup($type, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResourceGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **id** | **int**| Resource group ID |

### Return type

[**\Swagger\Client\Model\ResourceGroup**](../Model/ResourceGroup.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResourceUnit**
> \Swagger\Client\Model\ResourceUnit getResourceUnit($type, $id)

Returns a resource unit associated with the given id.

Returns a resource unit associated with the given id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$id = 56; // int | Resource unit ID

try {
    $result = $apiInstance->getResourceUnit($type, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResourceUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **id** | **int**| Resource unit ID |

### Return type

[**\Swagger\Client\Model\ResourceUnit**](../Model/ResourceUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResourceUnits**
> \Swagger\Client\Model\FilteredResourceUnitCollection getResourceUnits($type, $q)

Returns a set of resource units associated with the organization.

Returns a set of resource units associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$q = "q_example"; // string | Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language)

try {
    $result = $apiInstance->getResourceUnits($type, $q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResourceUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **q** | **string**| Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) | [optional]

### Return type

[**\Swagger\Client\Model\FilteredResourceUnitCollection**](../Model/FilteredResourceUnitCollection.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getResources**
> \Swagger\Client\Model\FilteredResourceCollection getResources($type, $q)

Returns a set of resources associated with the organization.

Returns a set of resources associated with the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | The type of resource
$q = "q_example"; // string | Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language)

try {
    $result = $apiInstance->getResources($type, $q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getResources: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| The type of resource |
 **q** | **string**| Filter collections with the [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) | [optional]

### Return type

[**\Swagger\Client\Model\FilteredResourceCollection**](../Model/FilteredResourceCollection.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getWaste**
> \Swagger\Client\Model\Waste getWaste($waste)

Returns a single waste item based on the given ID.

Returns a single waste item based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$waste = 56; // int | 

try {
    $result = $apiInstance->getWaste($waste);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getWaste: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **waste** | **int**|  |

### Return type

[**\Swagger\Client\Model\Waste**](../Model/Waste.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getWasteBooking**
> \Swagger\Client\Model\WasteBooking getWasteBooking($waste_booking)

Returns a waste booking associated with the given ID.

Returns a waste booking associated with the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$waste_booking = 56; // int | 

try {
    $result = $apiInstance->getWasteBooking($waste_booking);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getWasteBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **waste_booking** | **int**|  |

### Return type

[**\Swagger\Client\Model\WasteBooking**](../Model/WasteBooking.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getWastePerUnit**
> \Swagger\Client\Model\WastePerUnit getWastePerUnit($id)

Returns a single waste per unit based on the given ID.

Returns a single waste per unit based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getWastePerUnit($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getWastePerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\WastePerUnit**](../Model/WastePerUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getWasteUnit**
> \Swagger\Client\Model\WasteUnit getWasteUnit($id)

Returns a single waste unit based on the given ID.

Returns a single waste unit based on the given ID.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | 

try {
    $result = $apiInstance->getWasteUnit($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->getWasteUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |

### Return type

[**\Swagger\Client\Model\WasteUnit**](../Model/WasteUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **importMaterialPerUnits**
> importMaterialPerUnits($body, $supplier_id)

Creates material records based on the given material per unit import list if the data is unique.

Creates material records based on the given material per unit import list if the data is unique.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\MaterialPerUnitImportList(); // \Swagger\Client\Model\MaterialPerUnitImportList | 
$supplier_id = 56; // int | 

try {
    $apiInstance->importMaterialPerUnits($body, $supplier_id);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->importMaterialPerUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\MaterialPerUnitImportList**](../Model/MaterialPerUnitImportList.md)|  |
 **supplier_id** | **int**|  | [optional]

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **importWastePerUnits**
> importWastePerUnits($body)

Creates waste records based on the given waste per unit import list if the data is unique.

Creates waste records based on the given waste per unit import list if the data is unique.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\WastePerUnitImportList(); // \Swagger\Client\Model\WastePerUnitImportList | 

try {
    $apiInstance->importWastePerUnits($body);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->importWastePerUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\WastePerUnitImportList**](../Model/WastePerUnitImportList.md)|  |

### Return type

void (empty response body)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEquipment**
> \Swagger\Client\Model\EquipmentList listEquipment($q)

Returns a list of equipment items owned by the organization.

Returns a list of equipment items owned by the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEquipment($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listEquipment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EquipmentList**](../Model/EquipmentList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEquipmentBookings**
> \Swagger\Client\Model\EquipmentBookingList listEquipmentBookings($q)

Returns a list of equipment bookings made by the organization.

Returns a list of equipment bookings made by the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEquipmentBookings($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listEquipmentBookings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EquipmentBookingList**](../Model/EquipmentBookingList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEquipmentGroups**
> \Swagger\Client\Model\EquipmentGroupList listEquipmentGroups($q)

Returns a list of equipment groups owned by your organization.

Returns a list of equipment groups owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEquipmentGroups($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listEquipmentGroups: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EquipmentGroupList**](../Model/EquipmentGroupList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEquipmentPerUnit**
> \Swagger\Client\Model\EquipmentPerUnitList listEquipmentPerUnit($q)

Returns a bookable list of units associated with a piece of equipment.

Returns a bookable list of units associated with a piece of equipment.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEquipmentPerUnit($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listEquipmentPerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EquipmentPerUnitList**](../Model/EquipmentPerUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listEquipmentUnits**
> \Swagger\Client\Model\EquipmentUnitList listEquipmentUnits($q)

Returns a list of equipment units owned by your organization.

Returns a list of equipment units owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listEquipmentUnits($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listEquipmentUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\EquipmentUnitList**](../Model/EquipmentUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listGarbage**
> \Swagger\Client\Model\WasteList listGarbage($q)

Returns a list of waste owned by the organization.

Returns a list of waste owned by the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listGarbage($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listGarbage: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WasteList**](../Model/WasteList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listGarbageBookings**
> \Swagger\Client\Model\WasteBookingList listGarbageBookings($q)

Returns a list of waste bookings made by the organization.

Returns a list of waste bookings made by the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listGarbageBookings($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listGarbageBookings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WasteBookingList**](../Model/WasteBookingList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listGarbagePerUnit**
> \Swagger\Client\Model\WastePerUnitList listGarbagePerUnit($q)

Returns a bookable list of units associated with waste.

Returns a bookable list of units associated with waste.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listGarbagePerUnit($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listGarbagePerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WastePerUnitList**](../Model/WastePerUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMaterialBookings**
> \Swagger\Client\Model\MaterialBookingList listMaterialBookings($q)

Returns a list of material bookings made by the organization.

Returns a list of material bookings made by the organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listMaterialBookings($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listMaterialBookings: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\MaterialBookingList**](../Model/MaterialBookingList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMaterialUnits**
> \Swagger\Client\Model\MaterialUnitList listMaterialUnits($q)

Returns a list of material units owned by your organization.

Returns a list of materials units owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listMaterialUnits($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listMaterialUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\MaterialUnitList**](../Model/MaterialUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMaterials**
> \Swagger\Client\Model\MaterialList listMaterials($q)

Returns a list of materials owned by your organization.

Returns a list of materials owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listMaterials($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listMaterials: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\MaterialList**](../Model/MaterialList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listMaterialsPerUnit**
> \Swagger\Client\Model\MaterialPerUnitList listMaterialsPerUnit($q)

Returns a bookable list of units associated with materials.

Returns a bookable list of units associated with materials.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listMaterialsPerUnit($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listMaterialsPerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\MaterialPerUnitList**](../Model/MaterialPerUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listWaste**
> \Swagger\Client\Model\WasteList listWaste($q)

Returns a list of waste items owned by your organization.

Returns a list of waste items owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listWaste($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listWaste: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WasteList**](../Model/WasteList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listWastePerUnit**
> \Swagger\Client\Model\WastePerUnitList listWastePerUnit($q)

Returns a bookable list of units associated with waste.

Returns a bookable list of units associated with waste.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listWastePerUnit($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listWastePerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WastePerUnitList**](../Model/WastePerUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listWasteUnits**
> \Swagger\Client\Model\WasteUnitList listWasteUnits($q)

Returns a list of waste units owned by your organization.

Returns a list of waste units owned by your organization.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$q = "q_example"; // string | A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string

try {
    $result = $apiInstance->listWasteUnits($q);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->listWasteUnits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string**| A [Heimdall Query Language](https://heimdall.bouw7.nl/docs/query-language) string | [optional]

### Return type

[**\Swagger\Client\Model\WasteUnitList**](../Model/WasteUnitList.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postEquipment**
> \Swagger\Client\Model\Equipment postEquipment($body)

Create or update an equipment item.

Create or update the equipment item with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Equipment(); // \Swagger\Client\Model\Equipment | 

try {
    $result = $apiInstance->postEquipment($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postEquipment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Equipment**](../Model/Equipment.md)|  |

### Return type

[**\Swagger\Client\Model\Equipment**](../Model/Equipment.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postEquipmentBooking**
> \Swagger\Client\Model\EquipmentBooking postEquipmentBooking($body)

Create or update the equipment booking.

Create or update the equipment booking with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\EquipmentBooking(); // \Swagger\Client\Model\EquipmentBooking | 

try {
    $result = $apiInstance->postEquipmentBooking($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postEquipmentBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\EquipmentBooking**](../Model/EquipmentBooking.md)|  |

### Return type

[**\Swagger\Client\Model\EquipmentBooking**](../Model/EquipmentBooking.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postEquipmentGroup**
> \Swagger\Client\Model\EquipmentGroup postEquipmentGroup($body)

Creates or updates an equipment group for the currently authenticated user.

Creates or updates an equipment group for the currently authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\EquipmentGroup(); // \Swagger\Client\Model\EquipmentGroup | 

try {
    $result = $apiInstance->postEquipmentGroup($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postEquipmentGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\EquipmentGroup**](../Model/EquipmentGroup.md)|  |

### Return type

[**\Swagger\Client\Model\EquipmentGroup**](../Model/EquipmentGroup.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postEquipmentUnit**
> \Swagger\Client\Model\EquipmentUnit postEquipmentUnit($body)

Create or update the equipment unit.

Create or update the equipment unit with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\EquipmentUnit(); // \Swagger\Client\Model\EquipmentUnit | 

try {
    $result = $apiInstance->postEquipmentUnit($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postEquipmentUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\EquipmentUnit**](../Model/EquipmentUnit.md)|  |

### Return type

[**\Swagger\Client\Model\EquipmentUnit**](../Model/EquipmentUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postMaterial**
> \Swagger\Client\Model\Material postMaterial($body)

Create or update the material.

Create or update the material with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Material(); // \Swagger\Client\Model\Material | 

try {
    $result = $apiInstance->postMaterial($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Material**](../Model/Material.md)|  |

### Return type

[**\Swagger\Client\Model\Material**](../Model/Material.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postMaterialPerUnit**
> \Swagger\Client\Model\MaterialPerUnit postMaterialPerUnit($body)

Create or update the material per unit.

Create or update the material per unit with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\MaterialPerUnit(); // \Swagger\Client\Model\MaterialPerUnit | 

try {
    $result = $apiInstance->postMaterialPerUnit($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postMaterialPerUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\MaterialPerUnit**](../Model/MaterialPerUnit.md)|  |

### Return type

[**\Swagger\Client\Model\MaterialPerUnit**](../Model/MaterialPerUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postMaterialUnit**
> \Swagger\Client\Model\MaterialUnit postMaterialUnit($body)

Create or update the material unit.

Create or update the material unit with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\MaterialUnit(); // \Swagger\Client\Model\MaterialUnit | 

try {
    $result = $apiInstance->postMaterialUnit($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postMaterialUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\MaterialUnit**](../Model/MaterialUnit.md)|  |

### Return type

[**\Swagger\Client\Model\MaterialUnit**](../Model/MaterialUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postResource**
> \Swagger\Client\Model\Resource postResource($body)

Creates or updates a resource for the currently authenticated user.

Creates or updates a resource for the currently authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Resource(); // \Swagger\Client\Model\Resource | Resource object

try {
    $result = $apiInstance->postResource($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postResource: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Resource**](../Model/Resource.md)| Resource object |

### Return type

[**\Swagger\Client\Model\Resource**](../Model/Resource.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postResourceBooking**
> \Swagger\Client\Model\ResourceBooking postResourceBooking($body)

Creates or updates a resource booking for the currently authenticated user.

Creates or updates a resource booking for the currently authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceBooking(); // \Swagger\Client\Model\ResourceBooking | Resource booking object

try {
    $result = $apiInstance->postResourceBooking($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postResourceBooking: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceBooking**](../Model/ResourceBooking.md)| Resource booking object |

### Return type

[**\Swagger\Client\Model\ResourceBooking**](../Model/ResourceBooking.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postResourceGroup**
> \Swagger\Client\Model\ResourceGroup postResourceGroup($body)

Creates or updates a resource group for the currently authenticated user.

Creates or updates a resource group for the currently authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceGroup(); // \Swagger\Client\Model\ResourceGroup | 

try {
    $result = $apiInstance->postResourceGroup($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postResourceGroup: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceGroup**](../Model/ResourceGroup.md)|  |

### Return type

[**\Swagger\Client\Model\ResourceGroup**](../Model/ResourceGroup.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postResourceUnit**
> \Swagger\Client\Model\ResourceUnit postResourceUnit($body)

Creates or updates a resource unit for the currently authenticated user.

Creates or updates a resource unit for the currently authenticated user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\ResourceUnit(); // \Swagger\Client\Model\ResourceUnit | 

try {
    $result = $apiInstance->postResourceUnit($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postResourceUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ResourceUnit**](../Model/ResourceUnit.md)|  |

### Return type

[**\Swagger\Client\Model\ResourceUnit**](../Model/ResourceUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postWaste**
> \Swagger\Client\Model\Waste postWaste($body)

Create or update a waste item.

Create or update the waste item with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Waste(); // \Swagger\Client\Model\Waste | 

try {
    $result = $apiInstance->postWaste($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postWaste: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Waste**](../Model/Waste.md)|  |

### Return type

[**\Swagger\Client\Model\Waste**](../Model/Waste.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postWasteUnit**
> \Swagger\Client\Model\WasteUnit postWasteUnit($body)

Create or update the waste unit.

Create or update the waste unit with the schema.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ResourceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\WasteUnit(); // \Swagger\Client\Model\WasteUnit | 

try {
    $result = $apiInstance->postWasteUnit($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ResourceApi->postWasteUnit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\WasteUnit**](../Model/WasteUnit.md)|  |

### Return type

[**\Swagger\Client\Model\WasteUnit**](../Model/WasteUnit.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

