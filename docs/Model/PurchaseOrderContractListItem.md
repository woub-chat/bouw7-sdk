# PurchaseOrderContractListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**supplier** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**status** | **int** | Status of the contract | [optional] 
**status_name** | **string** | The name of the current status. | [optional] 
**type** | **int** | Type of the contract. (0 &#x3D; Permanent, 1 &#x3D; Directing) | [optional] 
**purchase_type** | **int** | The type of purchase. (2 &#x3D; Purchase Order, 4 &#x3D; Equipment, 5 &#x3D; Material, 6 &#x3D; Miscelaneous) | [optional] 
**delivery_address** | **string** | Delivery address of the purchase order contract. | [optional] 
**delivery_date** | **string** | Delivery date of the purchase order in ATOM-format. | [optional] 
**delivery_date_text** | **string** | Delivery date of the purchase order as free-form text. | [optional] 
**outstanding_costs** | **string** | Outstanding costs for the purchase order. | [optional] 
**current_approver** | **string** | The full name of the current approver. | [optional] 
**id** | **int** | The ID of the Contract. | [optional] 
**number** | **string** | The identification number of the contract. | [optional] 
**name** | **string** | The display name of the contract. Can be NULL. | [optional] 
**description** | **string** | The description of the contract. May contain HTML content. | [optional] 
**payment_agreement** | **string** | The payment agreement of the contract. May contain HTML content. | [optional] 
**linked_delivery_ticket** | [**\Swagger\Client\Model\NestedDeliveryTicketListItem**](NestedDeliveryTicketListItem.md) |  | [optional] 
**project_security_link** | [**\Swagger\Client\Model\NestedProjectSecurityCodeLinkListItem**](NestedProjectSecurityCodeLinkListItem.md) |  | [optional] 
**price** | **string** | The price of the contract. | [optional] 
**is_email_sent** | **bool** | True if an email was already sent. | [optional] 
**email_sent_at** | **string** | The date the email was sent in ATOM-format. | [optional] 
**email_sent_by** | **string** | The username of the user that sent the email. | [optional] 
**accepted_at** | **string** | The date when contract was accepted in ATOM-format. | [optional] 
**denied_at** | **string** | The date the contract was denied in ATOM-format. | [optional] 
**language** | **string** | The locale used by this contract, e.g.: nl-NL. | [optional] 
**attachment_count** | **int** | The attachment count for this contract. | [optional] 
**called_receipt_count** | **int** | The called receipt count for this contract. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


