# CustomAttributeListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this custom attribute. | [optional] 
**name** | **string** | The name of this custom attribute. | [optional] 
**property_name** | **string** | The name of the property as it will be displayed on associated list items. | [optional] 
**type** | **int** | The type of this field. (0 &#x3D; Text field, 1 &#x3D; Textarea, 2 &#x3D; Checkbox, 3 &#x3D; Date-picker, 4 &#x3D; Date-Time-picker, 6 &#x3D; Employee, 7 &#x3D; Contact) | [optional] 
**owner_type** | **int** | The type of owner this custom attribute should be associated with. (0 &#x3D; Project, 1 &#x3D; Contact, 2 &#x3D; Journal-day, 3 &#x3D; Employee) | [optional] 
**is_required** | **bool** | Whether this custom attribute is a required form field. | [optional] 
**is_read_only** | **bool** | Whether this custom attribute is a read-only field. | [optional] 
**is_visible_on_invoice** | **bool** | Whether this custom attribute is visible on invoices. | [optional] 
**is_visible_on_completion** | **bool** | Whether this custom attribute is visible on project completion. | [optional] 
**is_visible_on_hour_register** | **bool** | Whether this custom attribute is visible on hour register documents. | [optional] 
**is_visible_on_delivery** | **bool** | Whether this custom attribute is visible on delivery documents. | [optional] 
**is_visible_on_extra_work** | **bool** | Whether this custom attribute is visible on extra work documents. | [optional] 
**is_visible_on_garbage** | **bool** | Whether this custom attribute is visible on waste objects. | [optional] 
**is_visible_on_material** | **bool** | Whether this custom attribute is visible on material objects. | [optional] 
**is_visible_on_outsourcing** | **bool** | Whether this custom attribute is visible on outsourced objects. | [optional] 
**is_visible_on_checkout_document** | **bool** | Whether this custom attribute is visible on checkout documents. | [optional] 
**is_visible_on_qhse** | **bool** | Whether this custom attribute is visible on QHSE documents. | [optional] 
**is_visible_on_contract** | **bool** | Whether this custom attribute is visible on contracts. | [optional] 
**dropdown_values** | **string[]** | The dropdown values for the custom attribute. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


