# PendingApprovalListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this pending approval. | [optional] 
**type** | **int** | 0 &#x3D; Purchase invoice, 1 &#x3D; Purchase order, 2 &#x3D; Contract subcontractor. | [optional] 
**purchase_invoice_id** | **int** | Purchase invoice ID, can be null depends on the given type. | [optional] 
**purchase_order_contract_id** | **int** | Purchase order contract ID, can be null depends on the given type. | [optional] 
**subcontractor_contract_id** | **int** | Subcontractor contract ID, can be null depends on the given type. | [optional] 
**name** | **string** | Name of the contract or purchase invoice. | [optional] 
**number** | **string** | Number of the contract or purchase invoice. | [optional] 
**contact_name** | **string** | Contact name of the contact or purchase. | [optional] 
**project_name** | **string** | Project name of the contact or purchase. | [optional] 
**date** | **string** | The date contract or purchase invoice in ATOM format. | [optional] 
**status_id** | **int** | Status id of the contract or purchase invoice. | [optional] 
**cost_excluding_vat** | **int** | The cost excluding vat of the contract or purchase invoice. | [optional] 
**cost_including_vat** | **int** | The cost including vat of the contract or purchase invoice. | [optional] 
**comments** | **string** | The comment of the purchase invoice. | [optional] 
**book_number** | **string** | The booking number of the purchase invoice. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


