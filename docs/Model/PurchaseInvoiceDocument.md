# PurchaseInvoiceDocument

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of purchase invoice. | [optional] 
**is_booked** | **bool** | Whether the invoice is already booked. | [optional] 
**book_number** | **int** | The booknumber of the purchase invoice. | [optional] 
**invoice_number** | **string** | The invoice number of purchase invoice. | 
**order_number** | **string** | The order number of the purchase invoice. | [optional] 
**payment_reference** | **string** | The payment reference of the purchase invoice. | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | 
**branch** | [**\Swagger\Client\Model\CondensedBranch**](CondensedBranch.md) |  | [optional] 
**division** | [**\Swagger\Client\Model\CondensedDivision**](CondensedDivision.md) |  | [optional] 
**date** | **string** | Purchase invoice date. | 
**due_date** | **string** | Purchase invoice due date. | [optional] 
**exact_payment_condition** | **string** | The code of the Exact Online payment condition for this purchase invoice. | [optional] 
**date_paid** | **string** | Purchase invoice paid date. | [optional] 
**status** | **int** | Status of the purchase invoice. | 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | [optional] 
**delivery_ticket** | [**\Swagger\Client\Model\CondensedDeliveryTicket**](CondensedDeliveryTicket.md) |  | [optional] 
**comments** | **string** | Comment associated with the purchase invoice. | [optional] 
**lines** | [**\Swagger\Client\Model\PurchaseInvoiceDocumentLine[]**](PurchaseInvoiceDocumentLine.md) | The invoice lines associated with the purchase invoice. | [optional] 
**can_book_to_exact** | **bool** | Whether it is allowed to book to Exact. | [optional] 
**can_book_to_twinfield** | **bool** | Whether it is allowed to book to Twinfield. | [optional] 
**can_use_cost_center** | **bool** | True if the user can use cost center functionality. | [optional] 
**create_delivery_ticket** | **bool** | Whether or not to create a delivery ticket. | [optional] 
**create_delivery_ticket_for_remaining_costs** | **bool** | Whether or not to create a delivery ticket for the remaining costs. | [optional] 
**approval** | [**\Swagger\Client\Model\Approval**](Approval.md) |  | [optional] 
**g_account_amount** | **string** | The g account amount of the purchase invoice. | [optional] 
**previous_purchase_invoice_id** | **int** | The ID of the previous purchase invoice starting from this purchase invoice. Null when no previous purchase invoice available. | [optional] 
**next_purchase_invoice_id** | **int** | The ID of the next purchase invoice starting from this purchase invoice. Null when no next purchase invoice available. | [optional] 
**from_basecone** | **bool** | Whether the invoice is imported from Basecone. | [optional] 
**file** | [**\Swagger\Client\Model\File**](File.md) |  | [optional] 
**can_be_deleted** | **bool** | Whether the invoice can be deleted. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


