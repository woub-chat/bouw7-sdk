# QuotationListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the quotation. | [optional] 
**quotation_number** | **string** | The number of the quotation. | [optional] 
**subject** | **string** | The subject of the quotation. | [optional] 
**reference** | **string** | The reference of the quotation. | [optional] 
**quotation_date** | **string** | The date of the quotation, represented in ATOM-format. | [optional] 
**closing_chance** | **int** | The closing chance of this quotation. | [optional] 
**expected_closing_date** | **string** | The expected closing date of this quotation, represented in ATOM-format. | [optional] 
**commission_percentage** | **string** | The commission percentage of this quotation. | [optional] 
**salutation** | **int** | The salutation of this quotation. | [optional] 
**salutation_text** | **string** | The salutation text of the quotation. | [optional] 
**language** | **string** | The locale used by this quotation, e.g.: nl-NL. | [optional] 
**internal_note** | **string** | The internal note for this quotation. | [optional] 
**subtotal** | **string** | The sum of all quotation line subtotals, excluding VAT. | [optional] 
**total** | **string** | The sum of all quotation line subtotals, including VAT. | [optional] 
**employee** | [**\Swagger\Client\Model\NestedEmployeeListItem**](NestedEmployeeListItem.md) |  | [optional] 
**contact** | [**\Swagger\Client\Model\NestedContactListItem**](NestedContactListItem.md) |  | [optional] 
**branch** | [**\Swagger\Client\Model\NestedBranchListItem**](NestedBranchListItem.md) |  | [optional] 
**project** | [**\Swagger\Client\Model\NestedProjectListItem**](NestedProjectListItem.md) |  | [optional] 
**quotation_status** | [**\Swagger\Client\Model\NestedQuotationStatusListItem**](NestedQuotationStatusListItem.md) |  | [optional] 
**contact_person** | [**\Swagger\Client\Model\NestedContactPersonListItem**](NestedContactPersonListItem.md) |  | [optional] 
**contact_person_text** | **string** | The contact person text of the quotation. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


