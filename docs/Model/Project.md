# Project

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the project. | [optional] 
**parent_id** | **int** | The ID of the parent project if this project is a subproject. | [optional] 
**type** | **int** | The type of project. | 
**project_number** | **string** | The project number. | [optional] 
**full_project_number** | **string** | The full project number including year. | [optional] 
**division** | [**\Swagger\Client\Model\CondensedDivision**](CondensedDivision.md) |  | [optional] 
**is_booked** | **bool** | Whether or not the project has been booked to a bookkeeping system. | [optional] 
**name** | **string** | The name of the project. | [optional] 
**street_name** | **string** | The street name for the project. | [optional] 
**house_number** | **string** | The house number for the project. | [optional] 
**zip_code** | **string** | The zip code for the project. | [optional] 
**city** | **string** | The city of the project. | [optional] 
**country_code** | **string** | An ISO 3166-2 representation of the country. | [optional] 
**information** | **string** | Information about the project. | [optional] 
**planning** | **string** | The planning for the project. | [optional] 
**start_date** | **string** | Start date for the project in ATOM format. | [optional] 
**end_date** | **string** | End date for the project in ATOM format. | [optional] 
**delivery_date** | **string** | Delivery date for the project. | [optional] 
**extra_work** | **string** | Extra work for the project. | [optional] 
**hours_estimate** | **string** | Estimated hours for the project. | [optional] 
**hours_estimate_per_hour_types** | [**\Swagger\Client\Model\HoursEstimatePerHourType[]**](HoursEstimatePerHourType.md) | A list of HoursEstimatePerHourType schemas assigned to this project. | [optional] 
**fixed_price** | **string** | Fixed price for the project. | [optional] 
**general_costs_amount** | **string** | General costs amount for the project. | [optional] 
**additional_work** | **string** | Additional work amount for the project. | [optional] 
**profit_and_risk** | **string** | Profit and risk amount for the project. | [optional] 
**note** | **string** | Notes for the project. | [optional] 
**has_mareon_association** | **bool** | Whether or not the project has an association with Mareon. | [optional] 
**maintenance_status_code** | **string** | The maintenance status code for the project. | [optional] 
**is_security_coded** | **bool** | Whether or not the project is security coded. | [optional] 
**plan_item_count** | **int** | The count of plan items associated with this project. | [optional] 
**logged_hours** | **string** | The amount of hours logged for the project. | [optional] 
**branch** | [**\Swagger\Client\Model\CondensedBranch**](CondensedBranch.md) |  | [optional] 
**contact** | [**\Swagger\Client\Model\CondensedContact**](CondensedContact.md) |  | [optional] 
**category** | [**\Swagger\Client\Model\CondensedProjectCategory**](CondensedProjectCategory.md) |  | [optional] 
**contact_person** | [**\Swagger\Client\Model\CondensedContactPerson**](CondensedContactPerson.md) |  | [optional] 
**employees** | [**\Swagger\Client\Model\CondensedEmployee[]**](CondensedEmployee.md) | A list of condensed employee schemas assigned to this project. | [optional] 
**status** | [**\Swagger\Client\Model\CondensedProjectStatus**](CondensedProjectStatus.md) |  | 
**property_asset** | [**\Swagger\Client\Model\CondensedPropertyAsset**](CondensedPropertyAsset.md) |  | [optional] 
**custom_attribute_values** | [**\Swagger\Client\Model\CondensedCustomAttributeValue[]**](CondensedCustomAttributeValue.md) | A list of custom attribute values belonging to this project. | [optional] 
**reference** | **string** | A reference for this project. | [optional] 
**work_address** | **string** | The work address for this project. | [optional] 
**executor** | [**\Swagger\Client\Model\CondensedEmployee**](CondensedEmployee.md) |  | [optional] 
**work_planner** | [**\Swagger\Client\Model\CondensedEmployee**](CondensedEmployee.md) |  | [optional] 
**project_leader** | [**\Swagger\Client\Model\CondensedEmployee**](CondensedEmployee.md) |  | [optional] 
**created_at** | **string** | The creation time of the entity. | [optional] 
**created_by** | **string** | The user that created the entity. | [optional] 
**updated_at** | **string** | The last updated time of the entity. | [optional] 
**updated_by** | **string** | The user that last updated the entity. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


