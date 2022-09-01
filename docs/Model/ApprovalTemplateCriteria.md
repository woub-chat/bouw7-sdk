# ApprovalTemplateCriteria

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | ID of the criteria. | [optional] 
**name** | **string** | Name of the criteria. | 
**description** | **string** | Description of the criteria. | [optional] 
**workflow** | [**\Swagger\Client\Model\CondensedApprovalTemplateWorkflow**](CondensedApprovalTemplateWorkflow.md) |  | 
**type** | **int** | Criteria type. | 
**suppliers** | [**\Swagger\Client\Model\CondensedContact[]**](CondensedContact.md) | When using the priceLowerBound and or priceUpperBound the criteria will only conflict with criteria with the same supplier(s). | 
**branch** | [**\Swagger\Client\Model\CondensedBranch**](CondensedBranch.md) |  | [optional] 
**project_category** | [**\Swagger\Client\Model\CondensedProjectCategory**](CondensedProjectCategory.md) |  | [optional] 
**price_lower_bound** | **string** | The lower bound price of the criteria. The following &#39;operators&#39; are available:      *     cost &lt; priceUpperBound in psuedo: priceLowerBound is NULL and priceUpperBound is not NULL.      *     cost &gt; priceLowerBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NULL.      *     cost &#x3D; priceLowerBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NOT NULL and EQUAL to each other.      *     cost &gt; priceLowerBound and cost &lt; priceUpperBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NOT NULL and NOT EQUAL to each other.      * | [optional] 
**price_upper_bound** | **string** | The upper bound price of the criteria. The following &#39;operators&#39; are available:      *     cost &lt; priceUpperBound in psuedo: priceLowerBound is NULL and priceUpperBound is not NULL.      *     cost &gt; priceLowerBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NULL.      *     cost &#x3D; priceLowerBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NOT NULL and EQUAL to each other.      *     cost &gt; priceLowerBound and cost &lt; priceUpperBound in psuedo: priceLowerBound is NOT NULL and priceUpperBound is NOT NULL and NOT EQUAL to each other.      * | [optional] 
**delivery_ticket_matches_invoice_amount** | **bool** | Whether or not the delivery ticket price has to match the invoice amount. Only used in combination with type 0 (Purchase invoice). | 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


