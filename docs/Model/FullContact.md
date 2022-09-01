# FullContact

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of contact. | [optional] 
**name** | **string** | The contact name. | 
**street_name** | **string** | The street name of contact. | [optional] 
**house_number** | **string** | The house number (incl. additions). | [optional] 
**zip_code** | **string** | The zip-code. | [optional] 
**city** | **string** | The city name. | [optional] 
**country_code** | **string** | An ISO 3166-2 representation of the country. | [optional] 
**information** | **string** | Additional information about the contact. | [optional] 
**contact_person_name** | **string** | The name of person to contact. | [optional] 
**planning** | **string** | The planning text. | [optional] 
**coc_number** | **string** | The chamber of commerce number. | [optional] 
**vat_number** | **string** | The value added tax number. | [optional] 
**account_number** | **string** | The account number. | [optional] 
**hourly_rate** | **string** | The hourly rate. | [optional] 
**selling_hourly_rate** | **string** | The selling hourly rate. | [optional] 
**agreed_hourly_rate** | **string** | The agreed hourly rate. | [optional] 
**email** | **string** | The email address. | [optional] 
**phone_number** | **string** | The phone number. | [optional] 
**mobile_number** | **string** | The mobile phone number. | [optional] 
**gl_account_code_purchase** | **string** | A default general ledger account code to use for purchase related items. | [optional] 
**gl_account_code_invoice** | **string** | A default general ledger account code to use for invoice related items. | [optional] 
**debtor_number** | **string** | The debtor number. | [optional] 
**gln_number** | **string** | The Global Location Number. | [optional] 
**contact_type** | [**\Swagger\Client\Model\ContactType**](ContactType.md) |  | 
**is_vat_shifted** | **bool** | Whether VAT is shifted for the contact. | [optional] 
**n_account_text** | **string** | N-account text. | [optional] 
**wage_component_percentage** | **string** | Wage component percentage. | [optional] 
**g_account_text** | **string** | G-account text. | [optional] 
**g_account_percentage** | **string** | G-account percentage. | [optional] 
**expiration_reminder** | **int** | Expiration reminder days. | [optional] 
**invoice_mail** | **string** | The invoice mail. | [optional] 
**invoice_subject** | **string** | The invoice subject. | [optional] 
**reminder_mail** | **string** | The reminder mail. | [optional] 
**social_security_number** | **string** | The Social Security Number. | [optional] 
**first_reminder** | **int** | The first reminder. | [optional] 
**second_reminder** | **int** | The second reminder. | [optional] 
**surcharges** | [**\Swagger\Client\Model\Surcharges**](Surcharges.md) |  | [optional] 
**hour_type_prices** | [**\Swagger\Client\Model\HourTypePrice[]**](HourTypePrice.md) | A list of prices per hour types | [optional] 
**contact_divisions** | [**\Swagger\Client\Model\FullContactDivision[]**](FullContactDivision.md) | The linked divisions this contact is associated with. | [optional] 
**invoice_ubl_version** | **string** | The preferred UBL invoice version for this contact. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 
**custom_attribute_values** | [**\Swagger\Client\Model\CondensedCustomAttributeValue[]**](CondensedCustomAttributeValue.md) | A list of CustomAttributeValues belonging to the instance. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


