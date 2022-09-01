# PurchaseOrderContract

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the purchase order contract. | [optional] 
**supplier** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | 
**status** | **int** | Status of the contract. | 
**type** | **int** | Type of the contract. | 
**purchase_type** | **int** | The purchase type of the purchase order contract. | 
**delivery_address** | **string** | Delivery address of the purchase order contract. | 
**delivery_date** | **string** | Delivery date of the purchase order contract. | [optional] 
**delivery_date_text** | **string** | Delivery date text of the purchase order contract. | [optional] 
**called_receipts** | **int** | The amount of called receipt documents. | [optional] 
**log_entries** | **int** | The amount of log entries. | [optional] 
**contract_terms** | [**\Swagger\Client\Model\ContractTerm[]**](ContractTerm.md) | Contains the contract terms of this contract. | [optional] 
**approval** | [**\Swagger\Client\Model\Approval**](Approval.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | 
**number** | **string** | Number of the contract. | [optional] 
**contract_number** | **string** | The contract number of the contract. | [optional] 
**name** | **string** | The name of the contract. | [optional] 
**description** | **string** | The description of the contract. | [optional] 
**payment_agreement** | **string** | The payment agreement of the contract. | [optional] 
**linked_delivery_ticket** | [**\Swagger\Client\Model\CondensedDeliveryTicket**](CondensedDeliveryTicket.md) |  | [optional] 
**project_security_link** | [**\Swagger\Client\Model\CondensedProjectSecurityLink**](CondensedProjectSecurityLink.md) |  | [optional] 
**cost** | **string** | The cost of the contract. | 
**mail_sent** | **bool** | Flag to indicate if mail was sent. | [optional] 
**mail_sent_at** | **string** | The date the contract was sent. | [optional] 
**mail_sent_by** | **string** | The user that sent the email. | [optional] 
**accepted_at** | **string** | Datetime when contract was accepted. | [optional] 
**denied_at** | **string** | Datetime when contract was denied. | [optional] 
**language** | **string** | The locale used by this contract, e.g.: nl-NL. | [optional] 
**create_delivery_ticket** | **bool** | Whether or not to create a delivery ticket. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


