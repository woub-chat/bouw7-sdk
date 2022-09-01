# Quotation

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the quotation. | [optional] 
**employee** | [**\Swagger\Client\Model\CondensedEmployee**](CondensedEmployee.md) |  | 
**subject** | **string** | The subject of the quotation. | 
**reference** | **string** | The reference of the quotation. | [optional] 
**information** | **string** | The information of the quotation. | [optional] 
**footer** | **string** | The footer of the quotation. | [optional] 
**quotation_status** | [**\Swagger\Client\Model\CondensedQuotationStatus**](CondensedQuotationStatus.md) |  | 
**quotation_number** | **string** | The number of the quotation. | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | 
**contact_person** | [**\Swagger\Client\Model\ContactPerson**](ContactPerson.md) |  | [optional] 
**contact_person_text** | **string** | The contact person text of the quotation. | [optional] 
**salutation** | **int** | The salutation of this quotation. | [optional] 
**salutation_text** | **string** | The salutation text of the quotation. | [optional] 
**quotation_date** | **string** | The date of this quotation. | 
**expected_closing_date** | **string** | The expected closing date of this quotation. | [optional] 
**language** | **string** | The locale used by this quotation, e.g.: nl-NL. | 
**note** | **string** | The note of this quotation. | [optional] 
**mail_sent_at** | **string** | The date when the mail was sent. | [optional] 
**project** | [**\Swagger\Client\Model\CondensedProject**](CondensedProject.md) |  | [optional] 
**branch** | [**\Swagger\Client\Model\CondensedBranch**](CondensedBranch.md) |  | [optional] 
**disable_quotation_lines** | **bool** | Whether the quotation lines are disabled. | [optional] 
**conditions** | **string** | The conditions of this quotation. | [optional] 
**layout** | **string** | The layout of the quotation. | 
**show_price_per_line** | **bool** | Whether the price is shown per line. | [optional] 
**show_subtotal_per_chapter** | **bool** | Whether the subtotal is shown per chapter. | [optional] 
**show_total_price** | **bool** | Whether the total price is shown on this quotation. | [optional] 
**labour_day_price** | **string** | The labour day price of this quotation. | [optional] 
**calculation_labour_day_price** | **string** | The calculation labour day price of this quotation. | [optional] 
**discount** | **int** | The discount of this quotation. | [optional] 
**overheads** | **string** | The general costs of this quotation. | [optional] 
**overheads_vat_tariff** | [**\Swagger\Client\Model\CondensedVatTariff**](CondensedVatTariff.md) |  | [optional] 
**profit_and_risk** | **string** | The profit and risk costs of this quotation. | [optional] 
**profit_and_risk_vat_tariff** | [**\Swagger\Client\Model\CondensedVatTariff**](CondensedVatTariff.md) |  | [optional] 
**show_overheads_on_pdf** | **bool** | Whether the general costs and profit and risk should be shown on the quotation PDF. | [optional] 
**closing_chance** | **int** | The closing chance of this quotation. | [optional] 
**commission_percentage** | **string** | The commision percentage of this quotation. | [optional] 
**is_calculation** | **bool** | Whether the quotation is a calculation. | [optional] 
**activities_title** | **string** | The activities title of the quotation. | [optional] 
**attachments** | [**\Swagger\Client\Model\QuotationAttachment[]**](QuotationAttachment.md) |  | [optional] 
**common_attachments** | [**\Swagger\Client\Model\CommonQuotationAttachment[]**](CommonQuotationAttachment.md) |  | [optional] 
**chapters** | [**\Swagger\Client\Model\QuotationLineChapter[]**](QuotationLineChapter.md) |  | [optional] 
**sent_emails** | [**\Swagger\Client\Model\QuotationMail[]**](QuotationMail.md) | All mails sent for this invoice. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


