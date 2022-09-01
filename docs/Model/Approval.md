# Approval

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | ID of the approval. | [optional] 
**current_index** | **int** | The current index of the approver which turn it is to vote on the approval. | [optional] 
**workflow_id** | **int** | The workflow that this approval is based of. | [optional] 
**current_approver** | [**\Swagger\Client\Model\CondensedApprover**](CondensedApprover.md) |  | [optional] 
**last_action_date** | **string** | Date of the last action done to this approval. Will be null when no action has been made. | [optional] 
**is_approved** | **bool** | Whether or not the approval has been approved. | [optional] 
**can_approve** | **bool** | Whether or not the current authenticated user can approve the approval. | [optional] 
**approvers** | [**\Swagger\Client\Model\CondensedApprover[]**](CondensedApprover.md) | The approvers that must vote or already done so on this approval. | 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


