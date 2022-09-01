# EquipmentBooking

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the equipment booking. | [optional] 
**cost_price** | **string** | The cost price of the equipment booking. Can only be set on update. Initially set with the equipment per unit price. | [optional] 
**selling_price** | **string** | The selling price of the equipment booking. Can only be set on update. Initially set with the equipment per unit selling price. | [optional] 
**amount** | **string** | The amount of units of the equipment booking object. | 
**comment** | **string** | The comments for the equipment booking. | [optional] 
**log_date** | **string** | The log date of the equipment booking. | 
**project_security_link** | [**\Swagger\Client\Model\CondensedProjectSecurityLink**](CondensedProjectSecurityLink.md) |  | [optional] 
**equipment_per_unit** | [**\Swagger\Client\Model\CondensedEquipmentPerUnit**](CondensedEquipmentPerUnit.md) |  | 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | 
**employees** | [**\Swagger\Client\Model\CondensedEmployee[]**](CondensedEmployee.md) | The employees associated with this booking. | [optional] 
**equipment** | [**\Swagger\Client\Model\CondensedEquipment**](CondensedEquipment.md) |  | [optional] 
**equipment_group** | [**\Swagger\Client\Model\EquipmentGroup**](EquipmentGroup.md) |  | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


