# ProjectInvoiceTermListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | ID of the project invoice term. | [optional] 
**statement** | [**\Swagger\Client\Model\NestedProjectInvoiceTermStatementListItem**](NestedProjectInvoiceTermStatementListItem.md) |  | [optional] 
**description** | **string** | A description for the invoice term. | [optional] 
**percentage** | **string** | The percentage of the total sum this invoice term covers. | [optional] 
**subtotal** | **string** | The subtotal for this invoice term. | [optional] 
**invoiceable_at** | **string** | The date from which the term can be invoiced. | [optional] 
**vat_tariff_percentage** | **string** | The vat tariff percentage that was be applied to this term. | [optional] 
**vat_tariff** | [**\Swagger\Client\Model\NestedVatTariffListItem**](NestedVatTariffListItem.md) |  | [optional] 
**invoice_line** | [**\Swagger\Client\Model\NestedInvoiceLineListItem**](NestedInvoiceLineListItem.md) |  | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


