# Resource

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The unique identifier of the resource. | [optional] 
**type** | **string** | Resource type, possible values: equipment. | 
**code** | **string** | The code of the resource. | [optional] 
**name** | **string** | The name of the resource. | 
**description** | **string** | The description of the resource. | [optional] 
**inspection_date** | **string** | The inspection date of the resource. | [optional] 
**is_active** | **bool** | The active state of the resource. | [optional] 
**group** | [**\Swagger\Client\Model\CondensedResourceGroup**](CondensedResourceGroup.md) |  | 
**units** | [**\Swagger\Client\Model\ResourcePerUnit[]**](ResourcePerUnit.md) | The resource per unit. | [optional] 
**employees** | [**\Swagger\Client\Model\ResourceEmployee[]**](ResourceEmployee.md) | The resource employees. | [optional] 
**last_modified** | **string** | The last update time of the resource. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


