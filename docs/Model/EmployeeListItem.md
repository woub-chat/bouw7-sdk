# EmployeeListItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of this employee. | [optional] 
**first_name** | **string** | The given name of the employee. | [optional] 
**last_name** | **string** | The family name of the employee. | [optional] 
**department** | [**\Swagger\Client\Model\NestedDepartmentListItem**](NestedDepartmentListItem.md) |  | [optional] 
**email_address** | **string** | The email address of the employee. | [optional] 
**address** | **string** | The address, consisting of street name and house/building number, of the employee. | [optional] 
**zip_code** | **string** | The zip code, also known as postal code, associated with the address. | [optional] 
**city** | **string** | The city of residence of this employee. | [optional] 
**phone_number** | **string** | The phone number of the employee. | [optional] 
**birth_date** | **string** | The birth date of the employee. | [optional] 
**date_of_employment** | **string** | The employment date of the employee. | [optional] 
**date_of_resignation** | **string** | The resignation date of the employee. | [optional] 
**workload** | **string** | The amount of hours this employee is working on a weekly basis. | [optional] 
**hourly_rate** | **string** | The hourly rate. | [optional] 
**selling_hourly_rate** | **string** | The selling hourly rate. | [optional] 
**function_title** | **string** | The function title of this employee. | [optional] 
**external** | **bool** | True if employee is external, otherwise false. | [optional] 
**scab_id** | **string** | The scab ID of the employee. | [optional] 
**scab_employee_id** | **int** | The internal scab employee ID associated with this employee. | [optional] 
**user** | [**\Swagger\Client\Model\NestedUserLinkListItem**](NestedUserLinkListItem.md) |  | [optional] 
**avatar_file_hash** | **string** | The hash of the avatar/profile picture of this employee. | [optional] 
**has_signature** | **bool** | Wether the employee has a signature file configured. | [optional] 
**created_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**created_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 
**updated_by** | [**\Swagger\Client\Model\BlameableUser**](BlameableUser.md) |  | [optional] 
**updated_at** | **string** | The creation date of the object in ATOM/ISO-8601 format | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


