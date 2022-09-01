# EquipmentBookingListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this equipment booking. | [optional] 
**equipment** | [**\Swagger\Client\Model\NestedEquipmentPerUnitListItem**](NestedEquipmentPerUnitListItem.md) |  | [optional] 
**quantity** | **string** | The quantity of the booked item. | [optional] 
**cost_price** | **string** | The cost price of the booked item. | [optional] 
**selling_price** | **string** | The selling price of the booked item. | [optional] 
**total_cost_price** | **string** | The total cost price of the booked item. | [optional] 
**total_selling_price** | **string** | The total selling price of the booked item. | [optional] 
**invoiced_amount** | **string** | The invoiced amount of the booked item. | [optional] 
**date** | **string** | The log date of the booked item. | [optional] 
**comment** | **string** | The comment associated with this booked item. | [optional] 
**booking_status** | **int** | The status of this booking. 0 &#x3D; Registered, 1 &#x3D; Invoiced, 2 &#x3D; Not billable, 3 &#x3D; Credited. | [optional] 
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**project_security_link** | [**\Swagger\Client\Model\NestedProjectSecurityCodeLinkListItem**](NestedProjectSecurityCodeLinkListItem.md) |  | [optional] 
**invoice_line** | [**\Swagger\Client\Model\NestedInvoiceLineListItem**](NestedInvoiceLineListItem.md) |  | [optional] 
**booked_employee_names** | **string** | All employee names related to this equipment booking item, separated by a comma. | [optional] 
**equipment_group_id** | **string** | The equipment group ID related to this equipment booking item. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


