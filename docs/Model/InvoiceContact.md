# InvoiceContact

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the contact. | 
**name** | **string** | The name of the contact. | [optional] 
**contact_person_name** | **string** | The name of the contact person. | [optional] 
**street_name** | **string** | The street name of the contact. | [optional] 
**house_number** | **string** | The house- or building-number of the contact. | [optional] 
**zip_code** | **string** | The zip-code of the contact. | [optional] 
**city** | **string** | The city of residence of the contact. | [optional] 
**country** | **string** | The country of the contact. | [optional] 
**debtor_number** | **string** | The debtor number of the contact. | [optional] 
**iban** | **string** | The IBAN-account number of the contact. | [optional] 
**coc_number** | **string** | The chamber of commerce number of the contact. | [optional] 
**vat_number** | **string** | The VAT-number of the contact. | [optional] 
**email_address** | **string** | The email-address of the contact. | [optional] 
**phone_number** | **string** | The phone number of the contact. | [optional] 
**is_vat_shifted** | **bool** | Whether VAT is shifted for the contact. | [optional] 
**invoice_ubl_version** | **string** | The preferred UBL invoice version for this contact. | [optional] 
**n_account_text** | **string** | N-account text. | [optional] 
**wage_component_percentage** | **string** | Wage component percentage. | [optional] 
**g_account_text** | **string** | G-account text. | [optional] 
**g_account_percentage** | **string** | G-account percentage. | [optional] 
**custom_attribute_values** | [**\Swagger\Client\Model\CondensedCustomAttributeValue[]**](CondensedCustomAttributeValue.md) | A list of CustomAttributeValues belonging to this contact. | [optional] 
**expiration_reminder_days** | **int** | The number of days before a reminder is sent. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


