# EmployeeHourLogListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee** | [**\Swagger\Client\Model\NestedEmployeeListItem**](NestedEmployeeListItem.md) |  | [optional] 
**is_external** | **bool** | Whether the employee associated with this hour log entry is external. | [optional] 
**start_time** | **string** | The start time of the workday. Only available if enabled for your organization. | [optional] 
**end_time** | **string** | The end time of the workday. Only available if enabled for your organization. | [optional] 
**is_paid_off** | **bool** | Whether this price of this hour log entry has been paid off. | [optional] 
**is_scab_paid_off** | **bool** | Whether this price of this hour log entry has been paid off for scab users. | [optional] 
**id** | **int** | The ID of the hour log. | [optional] 
**booking_status** | **int** | The booking status of this entry. 0 &#x3D; Registered, 1 &#x3D; Invoiced, 2 &#x3D; Not billable, 3 &#x3D; Credited. | [optional] 
**type** | [**\Swagger\Client\Model\NestedHourTypeListItem**](NestedHourTypeListItem.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\NestedHourLogProjectListItem**](NestedHourLogProjectListItem.md) |  | [optional] 
**project_security_link** | [**\Swagger\Client\Model\NestedProjectSecurityCodeLinkListItem**](NestedProjectSecurityCodeLinkListItem.md) |  | [optional] 
**hours** | **string** | The amount of hours logged to this entry. | [optional] 
**log_date** | **string** | The log date of this entry. ATOM format. | [optional] 
**comment** | **string** | The remark added to this entry. | [optional] 
**hourly_rate** | **string** | The hourly rate. | [optional] 
**invoiced_amount** | **string** | The amount to invoice for this hour log entry. | [optional] 
**is_approved** | **bool** | Whether this hour log entry has been approved for processing. | [optional] 
**approved_by** | [**\Swagger\Client\Model\NestedUserListItem**](NestedUserListItem.md) |  | [optional] 
**approved_at** | **string** | The time this hour log entry was approved at. | [optional] 
**invoice_line** | [**\Swagger\Client\Model\NestedInvoiceLineListItem**](NestedInvoiceLineListItem.md) |  | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


