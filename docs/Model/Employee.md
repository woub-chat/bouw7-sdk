# Employee

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the employee. | [optional] 
**first_name** | **string** | The first name of the employee. | 
**last_name** | **string** | The last name of the employee. | 
**department** | [**\Swagger\Client\Model\CondensedDepartment**](CondensedDepartment.md) |  | 
**employee_mail** | **string** | The email of the employee. | [optional] 
**address** | **string** | The address of the employee. | [optional] 
**zip_code** | **string** | ZIP code of the address. | [optional] 
**city** | **string** | The city of the employee. | [optional] 
**phone_number** | **string** | The phone number of the employee. | [optional] 
**birth_date** | **string** | The birth date of the employee. | [optional] 
**workload** | **string** | The workload of the employee, this value is ignored when the workhour fields contain a value. | [optional] 
**hourly_rate** | **string** | The hourly rate | [optional] 
**selling_hourly_rate** | **string** | The selling hourly rate | [optional] 
**bsn** | **string** | The BSN of the employee. | [optional] 
**function** | **string** | The function of the employee. | [optional] 
**date_of_employment** | **string** | The date of employment of the employee in Y-m-d format. | [optional] 
**date_of_resignation** | **string** | The date of resignation of the employee in Y-m-d format. | [optional] 
**external** | **bool** | Whether the employee is external. | 
**afas_warehouse** | **string** | The warehouse material bookings of an employee will be booked on. Only applicable for AFAS. | [optional] 
**hour_type_prices** | [**\Swagger\Client\Model\HourTypePrice[]**](HourTypePrice.md) | A list of prices per hour types | [optional] 
**workhours_monday** | **string** | The standard amount of workhours on a monday. | [optional] 
**workhours_tuesday** | **string** | The standard amount of workhours on a tuesday. | [optional] 
**workhours_wednesday** | **string** | The standard amount of workhours on a wednesday. | [optional] 
**workhours_thursday** | **string** | The standard amount of workhours on a thursday. | [optional] 
**workhours_friday** | **string** | The standard amount of workhours on a friday. | [optional] 
**workhours_saturday** | **string** | The standard amount of workhours on a saturday. | [optional] 
**workhours_sunday** | **string** | The standard amount of workhours on a sunday. | [optional] 
**avatar_file_hash** | **string** | The hash of the avatar/profile picture of this employee. | [optional] 
**signature_file_hash** | **string** | The hash of the signature file of this employee. | [optional] 
**payroll_division** | [**\Swagger\Client\Model\CondensedDivision**](CondensedDivision.md) |  | [optional] 
**scab_id** | **string** | The external scab ID of the employee. | [optional] 
**scab_employee_id** | **int** | The internal ID of the Scab employee associated with this employee. | [optional] 
**username** | **string** | The username of the user associated with this employee. | [optional] 
**user_type** | **int** | The type of user associated with this employee. 0 &#x3D; None, 1 &#x3D; Admin, 2 &#x3D; Basic, 3 &#x3D; Platform. | [optional] 
**user_invitation_sent_at** | **string** | The invitation date of the user in ATOM/ISO-8601 format, for as long as the user has not accepted the invitation to this organization, NULL otherwise. | [optional] 
**user_activated_at** | **string** | The activation date of the user in ATOM/ISO-8601 format. | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 
**custom_attribute_values** | [**\Swagger\Client\Model\CondensedCustomAttributeValue[]**](CondensedCustomAttributeValue.md) | A list of CustomAttributeValues belonging to the instance. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


