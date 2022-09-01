# DeliveryTicket

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the delivery ticket. | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | 
**ticket_number** | **string** | Ticket number of the delivery ticket. | 
**ticket_date** | **string** | The date for which the delivery ticket were logged. | 
**purchase_type** | **int** | The purchase type. | 
**cost** | **string** | The costs for this delivery ticket. | [optional] 
**processed** | **bool** | Whether this delivery ticket is processed. | 
**description** | **string** | The description of this delivery ticket | [optional] 
**project_security_link** | [**\Swagger\Client\Model\CondensedProjectSecurityLink**](CondensedProjectSecurityLink.md) |  | [optional] 
**can_delete** | **bool** | Whether this delivery ticket can be deleted. | [optional] 
**initial_cost** | **string** | Initial cost of the delivery ticket. The value cannot be modified. | [optional] 
**file** | [**\Swagger\Client\Model\File**](File.md) |  | [optional] 
**purchase_invoice** | [**\Swagger\Client\Model\CondensedPurchaseInvoice**](CondensedPurchaseInvoice.md) |  | [optional] 
**contract** | [**\Swagger\Client\Model\CondensedContract**](CondensedContract.md) |  | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


