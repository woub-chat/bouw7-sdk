# DeliveryTicketListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this delivery ticket. | [optional] 
**number** | **string** | The ticket number of this delivery ticket. | [optional] 
**description** | **string** | The description of this delivery ticket. May contain HTML content. | [optional] 
**date** | **string** | The date of the delivery ticket, represented in ATOM-format. | [optional] 
**purchase_type_id** | **int** | The ID of the purchase type of this delivery ticket. | [optional] 
**purchase_type_name** | **string** | The name of the purchase type of this delivery ticket. | [optional] 
**price** | **string** | The price of this delivery ticket. | [optional] 
**is_processed** | **bool** | Whether this delivery ticket has been processed. | [optional] 
**booking_status** | **int** | The current booking status. 0 &#x3D; Registered, 1 &#x3D; Invoiced, 2 &#x3D; Not billable, 3 &#x3D; Credited. | [optional] 
**invoice_line** | [**\Swagger\Client\Model\NestedInvoiceLineListItem**](NestedInvoiceLineListItem.md) |  | [optional] 
**supplier** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**project_security_link** | [**\Swagger\Client\Model\NestedProjectSecurityCodeLinkListItem**](NestedProjectSecurityCodeLinkListItem.md) |  | [optional] 
**file_name** | **string** | The name of the file associated with the DeliveryTicket. | [optional] 
**file_hash** | **string** | The hash of the file associated with the DeliveryTicket. | [optional] 
**purchase_invoice_id** | **string** | The ID of the PurchaseInvoice associated with the DeliveryTicket. | [optional] 
**purchase_invoice_invoice_number** | **string** | The PurchaseInvoice invoice number associated with the DeliveryTicket. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


