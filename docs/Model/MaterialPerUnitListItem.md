# MaterialPerUnitListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this bookable unit. | [optional] 
**ean_code** | **string** | Ean code of this bookable unit. | [optional] 
**cost_price** | **string** | Cost price of this bookable unit. | [optional] 
**selling_price** | **string** | Selling price of this bookable unit. | [optional] 
**article_number** | **string** | The article number (usually EAN) of this bookable unit. | [optional] 
**unit** | [**\Swagger\Client\Model\NestedMaterialUnitListItem**](NestedMaterialUnitListItem.md) |  | [optional] 
**material** | [**\Swagger\Client\Model\NestedMaterialListItem**](NestedMaterialListItem.md) |  | [optional] 
**supplier** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**is_active** | **bool** | Whether this bookable unit is currently active. | [optional] 
**material_group** | [**\Swagger\Client\Model\NestedMaterialGroupListItem**](NestedMaterialGroupListItem.md) |  | [optional] 
**delivery_time_in_days** | **int** | The delivery time in days of this material per unit. | [optional] 
**conversion_factor** | **string** | The conversion factor of this material per unit. | [optional] 
**vat_tariff** | [**\Swagger\Client\Model\NestedVatTariffListItem**](NestedVatTariffListItem.md) |  | [optional] 
**visibility_flag** | **int** | The visibility flag of this material per unit. | [optional] 
**form_factor_type** | **int** | The type of the form factor associated with this material per unit. | [optional] 
**form_factor_unit** | **int** | The unit of the form factor associated with this material per unit. | [optional] 
**form_factor_sizes** | **string** | The sizes of the form factor associated with this material per unit. | [optional] 
**form_factor_weight** | **string** | The weight of the form factor associated with this material per unit. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


