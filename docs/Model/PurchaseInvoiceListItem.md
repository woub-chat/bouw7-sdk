# PurchaseInvoiceListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this purchase invoice. | [optional] 
**invoice_number** | **string** | The invoice number of this purchase invoice. | [optional] 
**payment_reference** | **string** | The payment reference of this purchase invoice. | [optional] 
**entry_number** | **int** | A sequential tracking number assigned to this purchase invoice. Also known as voucher number, serial number or tracking number. | [optional] 
**division** | [**\Swagger\Client\Model\NestedDivisionListItem**](NestedDivisionListItem.md) |  | [optional] 
**branch** | [**\Swagger\Client\Model\NestedBranchListItem**](NestedBranchListItem.md) |  | [optional] 
**current_approver** | **string** | The full name of the current approver. | [optional] 
**status** | **int** | The status of this purchase invoice. (0 &#x3D; New, 1 &#x3D; Approved, 2 &#x3D; Open, 3 &#x3D; Expired, 4 &#x3D; Paid, 5 &#x3D; Declined) | [optional] 
**comment** | **string** | A comment placed on this purchase invoice. | [optional] 
**order_number** | **string** | The order number associated with this purchase invoice. | [optional] 
**date** | **string** | The entry date of this purchase invoice. | [optional] 
**due_date** | **string** | The due date of this purchase invoice. | [optional] 
**date_paid** | **string** | The date this purchase invoice was paid. | [optional] 
**sub_total** | **string** | The sum of all purchase invoice line subtotals, excluding VAT. | [optional] 
**vat_total** | **string** | The sum of all purchase invoice line VAT totals. | [optional] 
**total** | **string** | The sum of all purchase invoice line subtotals, including VAT. | [optional] 
**supplier** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**delivery_ticket** | [**\Swagger\Client\Model\NestedDeliveryTicketListItem**](NestedDeliveryTicketListItem.md) |  | [optional] 
**is_booked_in_exact** | **bool** | Whether this purchase invoice is booked in Exact. | [optional] 
**is_booked_in_twinfield** | **bool** | Whether this purchase invoice is booked in Twinfield. | [optional] 
**is_originating_from_basecone** | **bool** | Whether this purchase invoice originates from Basecone. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


