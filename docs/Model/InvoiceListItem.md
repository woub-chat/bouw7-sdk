# InvoiceListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of invoice. | [optional] 
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**invoice_number** | **string** | The number of invoice. | [optional] 
**debtor_number** | **string** | The debtor number of the contact associated with this invoice. | [optional] 
**status** | **int** | The status of the invoice. (0 &#x3D; Open, 1 &#x3D; Expired, 2 &#x3D; Paid, 3 &#x3D; Draft) | [optional] 
**is_collective** | **bool** | Whether this is a collective invoice, containing lines associated with different projects. | [optional] 
**is_credit** | **bool** | Whether this is a credit invoice. | [optional] 
**division** | [**\Swagger\Client\Model\NestedDivisionListItem**](NestedDivisionListItem.md) |  | [optional] 
**branch** | [**\Swagger\Client\Model\NestedBranchListItem**](NestedBranchListItem.md) |  | [optional] 
**contact** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**contact_person_name** | **string** | The contact person for this invoice. Value can be NULL if undefined. | [optional] 
**date** | **string** | The invoice date in YYYY-MM-DD format, or NULL if the invoice date has not been set. | [optional] 
**date_paid** | **string** | The date when the invoice was paid in YYYY-MM-DD format, or NULL if the invoice is unpaid. | [optional] 
**sub_total** | **string** | The sum of all invoice line subtotals, excluding VAT. | [optional] 
**vat_total** | **string** | The sum of all invoice line VAT totals. | [optional] 
**total** | **string** | The sum of all invoice line subtotals, including VAT. | [optional] 
**is_booked_in_exact** | **bool** | Whether this invoice has been booked into your Exact administration. | [optional] 
**is_booked_in_twinfield** | **bool** | Whether this invoice has been booked into your Twinfield administration. | [optional] 
**is_booked_in_afas** | **bool** | Whether this invoice has been booked into your AFAS administration. | [optional] 
**is_booked_in_mareon** | **bool** | Whether this invoice has been booked into your Mareon administration. | [optional] 
**work_address** | **string** | The work address of this invoice. | [optional] 
**note** | **string** | The note of this invoice. | [optional] 
**is_mailed** | **bool** | Whether this invoice has been mailed. | [optional] 
**mail_date** | **string** | The date and time the invoice was mailed. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


