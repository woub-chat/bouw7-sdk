# CondensedPurchaseInvoice

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of purchase invoice. | [optional] 
**is_booked** | **bool** | Whether or not the purchase invoice has been booked to a bookkeeping system. | [optional] 
**can_be_deleted** | **bool** | Whether the invoice can be deleted. | [optional] 
**book_number** | **int** | The booknumber of the purchase invoice. | [optional] 
**order_number** | **int** | The order number of the purchase invoice. | [optional] 
**invoice_number** | **int** | The invoice number of purchase invoice. | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | [optional] 
**date** | **string** | Purchase invoice date. | [optional] 
**status** | **int** | Status of the purchase invoice. | [optional] 
**total_excluding_vat** | **string** | Price excluding VAT of the purchase invoice. | [optional] 
**total_including_vat** | **string** | Price including VAT of the purchase invoice. | [optional] 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | [optional] 
**delivery_ticket** | [**\Swagger\Client\Model\CondensedDeliveryTicket**](CondensedDeliveryTicket.md) |  | [optional] 
**comments** | **string** | Comment associated with the purchase invoice. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


