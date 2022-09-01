# InvoiceDocumentLine

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the invoice line. Must be omitted to create a new invoice. | [optional] 
**project_id** | **int** | The ID of the project associated with this invoice line. | [optional] 
**sort_index** | **int** | The sort index of this invoice line. | 
**linked_booking_items** | [**\Swagger\Client\Model\LinkedBookingItem[]**](LinkedBookingItem.md) | The linked booking items of this invoice line. | [optional] 
**project_invoice_term_id** | **int** | The ID of the project invoice term associated with this line. | [optional] 
**description** | **string** | The name of the invoice line. | 
**quantity** | **string** | The unit quantity of the invoice line. | 
**unit_name** | **string** | The name of the unit in the invoice line. | [optional] 
**unit_price** | **string** | The unit price of the invoice line. | 
**sub_total** | **string** | The sub-total price of the invoice line. | 
**surcharge_percentage** | **string** | The surcharge percentage of the invoice line. | [optional] 
**vat_tariff_percentage** | **string** | The VAT-tariff percentage used on the invoice line. Must be set to 0 if VAT is shifted. | [optional] 
**vat_tariff_id** | **int** | The VAT-tariff ID used on the invoice line. | 
**ledger** | **string** | A reference to the ledger of the invoice line. | [optional] 
**cost_center** | **string** | A reference to the cost center associated with the invoice line. | [optional] 
**reference** | **string** | Reference field of project (if available) from the invoice line. | [optional] 
**price_code** | **string** | The price code of the invoice line. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


