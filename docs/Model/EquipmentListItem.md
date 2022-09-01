# EquipmentListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this equipment. | [optional] 
**code** | **string** | The code of this equipment. | [optional] 
**name** | **string** | The name of this equipment. | [optional] 
**description** | **string** | The description of this equipment. | [optional] 
**inspection_date** | **string** | The last date of an inspection, in ATOM/ISO-8601 format. | [optional] 
**is_active** | **bool** | Whether this equipment is currently active / in service. | [optional] 
**group** | [**\Swagger\Client\Model\NestedEquipmentGroupListItem**](NestedEquipmentGroupListItem.md) |  | [optional] 
**is_current_user_assigned_by_default** | **bool** | Whether this current user is assigned by default. | [optional] 
**associated_unit_names** | **string** | All unit names related to this equipment item. | [optional] 
**associated_employee_names** | **string** | All employee full names related to this equipment item. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


