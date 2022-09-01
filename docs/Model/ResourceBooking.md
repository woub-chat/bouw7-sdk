# ResourceBooking

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The unique identifier of the resource booking. | [optional] 
**type** | **string** | Resource type, possible values: equipment. | 
**project** | [**\Swagger\Client\Model\ResourceBookingProjectInfo**](ResourceBookingProjectInfo.md) |  | 
**project_security_link** | [**\Swagger\Client\Model\ResourceProjectSecurityLink**](ResourceProjectSecurityLink.md) |  | [optional] 
**resource** | [**\Swagger\Client\Model\ResourceBookingInfo**](ResourceBookingInfo.md) |  | [optional] 
**group** | [**\Swagger\Client\Model\ResourceGroupBookingInfo**](ResourceGroupBookingInfo.md) |  | [optional] 
**unit** | [**\Swagger\Client\Model\ResourceUnitBookingInfo**](ResourceUnitBookingInfo.md) |  | 
**amount** | **string** | The amount of the resource booking. | 
**price** | **string** | The price of this booking, if this is not provided, the price of the unit will be used for the booking. | [optional] 
**price_total** | **string** | The total price of this booking. | [optional] 
**selling_price** | **string** | The selling price of this booking. | [optional] 
**selling_price_total** | **string** | The total selling price of this booking. | [optional] 
**log_date** | **string** | The cost price of this booking. | 
**comment** | **string** | The comment of this booking. | [optional] 
**employees** | [**\Swagger\Client\Model\ResourceEmployee[]**](ResourceEmployee.md) | The employees of this booking. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


