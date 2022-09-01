# ProjectInvoiceTerm

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the invoice term. | [optional] 
**invoice_line** | [**\Swagger\Client\Model\CondensedInvoiceLine**](CondensedInvoiceLine.md) |  | [optional] 
**description** | **string** | A description for this invoice term. | 
**percentage** | **string** | The percentage of the total sum this invoice term covers. | 
**subtotal** | **string** | The subtotal for this invoice term. | 
**vat_tariff_percentage** | **string** | The vat tariff percentage that was applied to this invoice term. | [optional] 
**vat_tariff_object** | [**\Swagger\Client\Model\CondensedVatTariff**](CondensedVatTariff.md) |  | 
**invoiceable_at** | **string** | The date from which the term can be invoiced. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


