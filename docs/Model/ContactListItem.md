# ContactListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of contact. | [optional] 
**name** | **string** | The contact name. | [optional] 
**street_name** | **string** | The street name of contact. | [optional] 
**house_number** | **string** | The house number (incl. additions). | [optional] 
**address** | **string** | The address. | [optional] 
**zip_code** | **string** | The zip-code. | [optional] 
**city** | **string** | The city name. | [optional] 
**country_code** | **string** | An ISO 3166-2 representation of the country. | [optional] 
**information** | **string** | Additional information about the contact. | [optional] 
**contact_person_name** | **string** | The name of the financial contact person, Primarily used for invoicing purposes. | [optional] 
**planning_text** | **string** | The planning text. | [optional] 
**coc_number** | **string** | The chamber of commerce number. | [optional] 
**vat_number** | **string** | The value added tax number. | [optional] 
**iban** | **string** | The IBAN account number. | [optional] 
**hourly_rate** | **string** | The hourly rate. | [optional] 
**selling_hourly_rate** | **string** | The selling hourly rate. | [optional] 
**agreed_hourly_rate** | **string** | The agreed hourly rate. | [optional] 
**email_address** | **string** | The email address. | [optional] 
**invoice_mail** | **string** | The invoice email address. | [optional] 
**reminder_mail** | **string** | The reminder email address. | [optional] 
**invoice_subject** | **string** | The invoice subject. | [optional] 
**invoice_ubl_version** | **string** | The invoice ubl version. | [optional] 
**phone_number** | **string** | The phone number. | [optional] 
**mobile_phone_number** | **string** | The mobile phone number. | [optional] 
**debtor_number** | **string** | The debtor number. Only used if the organization has no divisions. | [optional] 
**gln_number** | **string** | The Global Location Number. | [optional] 
**expiration_reminder** | **int** | The expiration reminder days. | [optional] 
**type** | [**\Swagger\Client\Model\NestedContactTypeListItem**](NestedContactTypeListItem.md) |  | [optional] 
**is_vat_shifted** | **bool** | True if VAT is shifted from the invoice. | [optional] 
**n_account_text** | **string** | N-account text. | [optional] 
**wage_component_percentage** | **string** | Wage component percentage. | [optional] 
**g_account_text** | **string** | G-account text. | [optional] 
**g_account_percentage** | **string** | G-account percentage. | [optional] 
**associated_property_asset_names** | **string** | All property asset names related to this contact. | [optional] 
**has_accounting_software** | **bool** | Whether the contact has either Exact or Twinfield accounting software. Not applicable if the organization has divisions. | [optional] 
**debtor_numbers** | **string** | The deptor numbers for each contact division associated with the contact. Only available if the organization has divisions. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


