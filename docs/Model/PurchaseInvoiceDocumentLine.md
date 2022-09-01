# PurchaseInvoiceDocumentLine

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the purchase invoice line. Must be omitted to create a new purchase invoice line. | [optional] 
**description** | **string** | The description of the purchase invoice line. | 
**quantity** | **string** | The unit quantity of the purchase invoice line. | 
**unit_name** | **string** | The name of the unit in the purchase invoice line. | [optional] 
**unit_price** | **string** | The unit price of the purchase invoice line. | 
**gross_price** | **string** | The gross price of the purchase invoice line. | [optional] 
**sub_total** | **string** | The sub-total price of the purchase invoice line. | 
**vat_tariff_percentage** | **string** | The VAT-tariff percentage used on the purchase invoice line. Must be set to 0 if VAT is shifted. | [optional] 
**vat_tariff_id** | **int** | The VAT-tariff ID used on the purchase invoice line. | 
**ledger** | **string** | A reference to the ledger of the purchase invoice line. | [optional] 
**cost_center** | **string** | A reference to the cost center associated with the invoice line. | [optional] 
**delivery_ticket** | [**\Swagger\Client\Model\DeliveryTicketWithProjectDetails**](DeliveryTicketWithProjectDetails.md) |  | [optional] 
**model_id** | **int** | The model ID. Will be the ID of the selected modelType. | [optional] 
**model_type** | **int** | The model type, possible options: 1 &#x3D; SubcontractorContract / 2 &#x3D; PurchaseOrderContract / 3 &#x3D; Project. | [optional] 
**create_delivery_ticket_for_remaining_costs** | **bool** | Whether or not to create a delivery ticket for remaining costs between this line and the delivery ticket | [optional] 
**can_be_edited** | **bool** | Whether the line can be edited or removed. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


