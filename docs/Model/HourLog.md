# HourLog

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the hour log. | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | [optional] 
**employee** | [**\Swagger\Client\Model\CondensedEmployee**](CondensedEmployee.md) |  | [optional] 
**log_hours** | **string** | The amount of hours logged. | 
**invoice_amount** | **string** | The amount that will be shown on the invoice. | [optional] 
**log_date** | **string** | The date for which the hours were logged. | 
**start_time** | **string** | The start time of the workday. Only available if enabled for your organization. | [optional] 
**end_time** | **string** | The end time of the workday. Only available if enabled for your organization. | [optional] 
**hour_type** | [**\Swagger\Client\Model\CondensedHourType**](CondensedHourType.md) |  | 
**comments** | **string** | The comments for this hour log. | [optional] 
**hourly_rate** | **string** | The hourly rate. | [optional] 
**approved** | **bool** | Whether this hour log has been approved. | [optional] 
**paid_off** | **bool** | Whether this hour log has been paid off. | [optional] 
**project_security_link** | [**\Swagger\Client\Model\CondensedProjectSecurityLink**](CondensedProjectSecurityLink.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


