# Bouw7 SDK client
- API version: 1.0.0


## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/pawas007/bouw7-sdk.git"
    }
  ],
  "require": {
    "/": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ApprovalApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CondensedApprovalTemplateCriteria(); // \Swagger\Client\Model\CondensedApprovalTemplateCriteria | 

try {
    $apiInstance->deleteApprovalCriteria($body);
} catch (Exception $e) {
    echo 'Exception when calling ApprovalApi->deleteApprovalCriteria: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://heimdall.bouw7.nl*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ApprovalApi* | [**deleteApprovalCriteria**](docs/Api/ApprovalApi.md#deleteapprovalcriteria) | **DELETE** /approval-template/criteria | Delete the given approval criteria.
*ApprovalApi* | [**deleteApprovalWorkflow**](docs/Api/ApprovalApi.md#deleteapprovalworkflow) | **DELETE** /approval-template/workflow | Delete the given approval workflow.
*ApprovalApi* | [**findDefaultApprovalSettings**](docs/Api/ApprovalApi.md#finddefaultapprovalsettings) | **GET** /approval-template/default-settings | Find the default approval settings for the current organization.
*ApprovalApi* | [**findMatchingApprovalCriteria**](docs/Api/ApprovalApi.md#findmatchingapprovalcriteria) | **POST** /approval-template/match-criteria | Find the matching approval workflow based on the criteria with the highest score for the given schema.
*ApprovalApi* | [**getApprovalTemplateCriteria**](docs/Api/ApprovalApi.md#getapprovaltemplatecriteria) | **GET** /approval-template/criteria/{id} | Returns a single approval template criteria based on the given ID.
*ApprovalApi* | [**getApprovalTemplateWorkflow**](docs/Api/ApprovalApi.md#getapprovaltemplateworkflow) | **GET** /approval-template/workflow/{id} | Returns a single approval template workflow based on the given ID, duplicate approvers are not filtered out!
*ApprovalApi* | [**getCriteriaTypes**](docs/Api/ApprovalApi.md#getcriteriatypes) | **GET** /approval-template/criteria-types | Retrieve all approval template criteria types.
*ApprovalApi* | [**getWorkflowTypes**](docs/Api/ApprovalApi.md#getworkflowtypes) | **GET** /approval-template/workflow-types | Retrieve all possible types with sub-types for an approval workflow.
*ApprovalApi* | [**listApprovalCriteria**](docs/Api/ApprovalApi.md#listapprovalcriteria) | **GET** /list/approval-template/criteria | Return a list of all approval criteria associated with the organization.
*ApprovalApi* | [**listApprovalWorkflows**](docs/Api/ApprovalApi.md#listapprovalworkflows) | **GET** /list/approval-template/workflows | Returns a list of approval workflows for the organization of the current authenticated user. Use HQL to filter for specific items.
*ApprovalApi* | [**listPendingApprovalsAssignedToMe**](docs/Api/ApprovalApi.md#listpendingapprovalsassignedtome) | **GET** /list/approval/assigned-to-me | List all pending approvals for the current authenticated user.
*ApprovalApi* | [**postApprovalCriteria**](docs/Api/ApprovalApi.md#postapprovalcriteria) | **POST** /approval-template/criteria | Create or update the approval criteria with the schema.
*ApprovalApi* | [**postDefaultApprovalSettings**](docs/Api/ApprovalApi.md#postdefaultapprovalsettings) | **POST** /approval-template/default-settings | Update the default approval settings for the current organization.
*ApprovalApi* | [**postWorkflow**](docs/Api/ApprovalApi.md#postworkflow) | **POST** /approval-template/workflow | Create or update the approval workflow with the schema.
*ApprovalApi* | [**voteOnContract**](docs/Api/ApprovalApi.md#voteoncontract) | **POST** /approval/{approval}/vote-on-contract | Vote on a contract approval.
*ApprovalApi* | [**voteOnPurchaseInvoice**](docs/Api/ApprovalApi.md#voteonpurchaseinvoice) | **POST** /approval/{approval}/vote-on-purchase-invoice | Vote on a purchase invoice approval.
*AuditLogApi* | [**getPurchaseInvoiceAuditLogs**](docs/Api/AuditLogApi.md#getpurchaseinvoiceauditlogs) | **GET** /purchase-invoice/{purchaseInvoice}/audit-logs | Get all purchase invoice audit logs.
*AuditLogApi* | [**getQuotationAuditLogs**](docs/Api/AuditLogApi.md#getquotationauditlogs) | **GET** /quotation/{quotation}/audit-logs | Get all Quotation audit logs.
*BookingApi* | [**findBookingLines**](docs/Api/BookingApi.md#findbookinglines) | **GET** /project/{project}/booking-lines | Returns all available booking items based on its criteria.
*CalendarApi* | [**deleteDayOff**](docs/Api/CalendarApi.md#deletedayoff) | **DELETE** /day-off | Delete the given day off.
*CalendarApi* | [**deleteDayOffPerEmployee**](docs/Api/CalendarApi.md#deletedayoffperemployee) | **DELETE** /organization/day-off-per-employee | Delete the given day off per employee.
*CalendarApi* | [**getDayOff**](docs/Api/CalendarApi.md#getdayoff) | **GET** /day-off/{id} | Returns a single day off based on the given ID.
*CalendarApi* | [**getDayOffPerEmployee**](docs/Api/CalendarApi.md#getdayoffperemployee) | **GET** /organization/day-off-per-employee/{id} | Returns a single day off per employee based on the given ID.
*CalendarApi* | [**listDaysOff**](docs/Api/CalendarApi.md#listdaysoff) | **GET** /list/days-off | Returns a list of holidays / non-working days.
*CalendarApi* | [**listDaysOffPerEmployee**](docs/Api/CalendarApi.md#listdaysoffperemployee) | **GET** /list/days-off-per-employee | Returns a list of day off per employee schemas associated with the organization.
*CalendarApi* | [**postDayOff**](docs/Api/CalendarApi.md#postdayoff) | **POST** /day-off | Create or update the day off.
*CalendarApi* | [**postDayOffPerEmployee**](docs/Api/CalendarApi.md#postdayoffperemployee) | **POST** /organization/day-off-per-employee | Create or update the day off per employee.
*ContactApi* | [**deleteContact**](docs/Api/ContactApi.md#deletecontact) | **DELETE** /contact | Delete the given contact.
*ContactApi* | [**deleteContactPerson**](docs/Api/ContactApi.md#deletecontactperson) | **DELETE** /contact/{contact}/contact-person | Delete the given contact person.
*ContactApi* | [**getContact**](docs/Api/ContactApi.md#getcontact) | **GET** /contact/{id} | Returns a single contact based on the given ID.
*ContactApi* | [**getContactPerson**](docs/Api/ContactApi.md#getcontactperson) | **GET** /contact-person/{id} | Returns a single contact person based on the given ID.
*ContactApi* | [**getContactTypes**](docs/Api/ContactApi.md#getcontacttypes) | **GET** /contact-types | Retrieves a list of contact types.
*ContactApi* | [**getSurchargePercentages**](docs/Api/ContactApi.md#getsurchargepercentages) | **GET** /contact/{contact}/surcharge-percentages | 
*ContactApi* | [**listContactFinancial**](docs/Api/ContactApi.md#listcontactfinancial) | **GET** /list/contact/financial | Returns a list of financial contact details associated with the organization.
*ContactApi* | [**listContactPersons**](docs/Api/ContactApi.md#listcontactpersons) | **GET** /list/contact-persons | Returns a list of contact persons associated with any contact for your organization.
*ContactApi* | [**listContacts**](docs/Api/ContactApi.md#listcontacts) | **GET** /list/contacts | Returns a list of contacts associated with the organization.
*ContactApi* | [**postContact**](docs/Api/ContactApi.md#postcontact) | **POST** /contact | Create or update the contact.
*ContactApi* | [**postContactPerson**](docs/Api/ContactApi.md#postcontactperson) | **POST** /contact/{contact}/contact-person | Create or update the contact person for the given contact.
*ContractApi* | [**deleteContractOrderLine**](docs/Api/ContractApi.md#deletecontractorderline) | **DELETE** /project/{project}/contract-order-line | Delete the given contract order line.
*ContractApi* | [**deletePurchaseOrder**](docs/Api/ContractApi.md#deletepurchaseorder) | **DELETE** /contracts/purchase-order | Delete the given purchase order contract.
*ContractApi* | [**deletePurchaseOrderContractTerm**](docs/Api/ContractApi.md#deletepurchaseordercontractterm) | **DELETE** /contracts/purchase-order/contract-term | Delete the given purchase order contract term.
*ContractApi* | [**deleteSubcontractor**](docs/Api/ContractApi.md#deletesubcontractor) | **DELETE** /contracts/subcontractor | Delete the given subcontractor contract.
*ContractApi* | [**deleteSubcontractorContractTerm**](docs/Api/ContractApi.md#deletesubcontractorcontractterm) | **DELETE** /contracts/subcontractor/contract-term | Delete the given subcontractor contract term.
*ContractApi* | [**getCalledReceiptBySubcontractorContract**](docs/Api/ContractApi.md#getcalledreceiptbysubcontractorcontract) | **GET** /contracts/subcontractor/called-receipts/{id} | Returns a list of subcontractor contract called receipts associated with the given ID.
*ContractApi* | [**getCalledReceiptsByPurchaseOrderContract**](docs/Api/ContractApi.md#getcalledreceiptsbypurchaseordercontract) | **GET** /contracts/purchase-order/called-receipts/{id} | Returns a list of purchase order contract called receipts associated with the given ID.
*ContractApi* | [**getFilesByPurchaseOrderContract**](docs/Api/ContractApi.md#getfilesbypurchaseordercontract) | **GET** /contracts/purchase-order/files/{id} | Returns a collection of purchase order contract files with the given ID.
*ContractApi* | [**getFilesBySubcontractorContract**](docs/Api/ContractApi.md#getfilesbysubcontractorcontract) | **GET** /contracts/subcontractor/files/{id} | Returns a collection of subcontractor contract files with the given ID.
*ContractApi* | [**getPurchaseOrder**](docs/Api/ContractApi.md#getpurchaseorder) | **GET** /contracts/purchase-order/{id} | Returns a single purchase order contract based on the given ID.
*ContractApi* | [**getPurchaseOrderContractHistoryEntries**](docs/Api/ContractApi.md#getpurchaseordercontracthistoryentries) | **GET** /contracts/purchase-order/log-entries/{id} | Returns a list of purchase order contract history entries associated with the given ID.
*ContractApi* | [**getPurchaseOrderCostTypes**](docs/Api/ContractApi.md#getpurchaseordercosttypes) | **GET** /contracts/purchase-order/cost-types | Returns available cost types for a purchase order.
*ContractApi* | [**getPurchaseOrderStatuses**](docs/Api/ContractApi.md#getpurchaseorderstatuses) | **GET** /contracts/purchase-order/statuses | Returns available statuses for a purchase order.
*ContractApi* | [**getSubcontractor**](docs/Api/ContractApi.md#getsubcontractor) | **GET** /contracts/subcontractor/{id} | Returns a single subcontractor contract based on the given ID.
*ContractApi* | [**getSubcontractorContractHistoryEntries**](docs/Api/ContractApi.md#getsubcontractorcontracthistoryentries) | **GET** /contracts/subcontractor/log-entries/{id} | Returns a list of subcontractor contract history entries associated with the given ID.
*ContractApi* | [**getSubcontractorStatuses**](docs/Api/ContractApi.md#getsubcontractorstatuses) | **GET** /contracts/subcontractor/statuses | Returns available statuses for a subcontractor contract.
*ContractApi* | [**listContractOrderLines**](docs/Api/ContractApi.md#listcontractorderlines) | **GET** /list/contract-order-lines | Returns all contract order lines for the current organization. Use HQL to filter for specific items.
*ContractApi* | [**listPurchaseOrderContractTerms**](docs/Api/ContractApi.md#listpurchaseordercontractterms) | **GET** /list/purchase-order-contract-terms | Returns a list of purchase order contract terms.
*ContractApi* | [**listPurchaseOrderContracts**](docs/Api/ContractApi.md#listpurchaseordercontracts) | **GET** /list/purchase-order-contracts | Returns a list of purchase order contracts.
*ContractApi* | [**listSubcontractorContractTerms**](docs/Api/ContractApi.md#listsubcontractorcontractterms) | **GET** /list/subcontractor-contract-terms | Returns a list of subcontractor contract terms.
*ContractApi* | [**listSubcontractorContracts**](docs/Api/ContractApi.md#listsubcontractorcontracts) | **GET** /list/subcontractor-contracts | Returns a list of subcontractor contracts.
*ContractApi* | [**postContractOrderLine**](docs/Api/ContractApi.md#postcontractorderline) | **POST** /project/{project}/contract-order-line | Create or update the contract order line.
*ContractApi* | [**postPurchaseOrder**](docs/Api/ContractApi.md#postpurchaseorder) | **POST** /contracts/purchase-order | Create or update a purchase order contract with the schema.
*ContractApi* | [**postPurchaseOrderContractTerm**](docs/Api/ContractApi.md#postpurchaseordercontractterm) | **POST** /contracts/purchase-order/contract-term | Create or update the purchase order contract term.
*ContractApi* | [**postSubcontractor**](docs/Api/ContractApi.md#postsubcontractor) | **POST** /contracts/subcontractor | Create or update a subcontractor contract with the schema.
*ContractApi* | [**postSubcontractorContractTerm**](docs/Api/ContractApi.md#postsubcontractorcontractterm) | **POST** /contracts/subcontract/contract-term | Create or update the subcontractor contract term.
*ContractApi* | [**updatePurchaseOrderStatus**](docs/Api/ContractApi.md#updatepurchaseorderstatus) | **PUT** /contracts/purchase-order/{id}/update-status/{status} | Update the purchase order contract with the given status.
*ContractApi* | [**updateSubcontractorStatus**](docs/Api/ContractApi.md#updatesubcontractorstatus) | **PUT** /contracts/subcontractor/{id}/update-status/{status} | Update the subcontractor contract with the given status.
*DeliveryTicketApi* | [**deleteDeliveryTicket**](docs/Api/DeliveryTicketApi.md#deletedeliveryticket) | **DELETE** /project/delivery-ticket | Delete the given delivery ticket.
*DeliveryTicketApi* | [**getDeliveryTicket**](docs/Api/DeliveryTicketApi.md#getdeliveryticket) | **GET** /project/delivery-ticket/{id} | Returns a single delivery ticket based on the given ID.
*DeliveryTicketApi* | [**getPurchaseTypes**](docs/Api/DeliveryTicketApi.md#getpurchasetypes) | **GET** /delivery-ticket/purchase-types | Returns available purchase types for a delivery ticket.
*DeliveryTicketApi* | [**listDeliveryTickets**](docs/Api/DeliveryTicketApi.md#listdeliverytickets) | **GET** /list/delivery-tickets | Returns a list of delivery tickets associated with your organization.
*DeliveryTicketApi* | [**postDeliveryTicket**](docs/Api/DeliveryTicketApi.md#postdeliveryticket) | **POST** /project/delivery-ticket | Create or update the delivery ticket.
*DepartmentApi* | [**deleteDepartment**](docs/Api/DepartmentApi.md#deletedepartment) | **DELETE** /organization/department | Delete the given department.
*DepartmentApi* | [**deleteDepartmentWorkInProgressSettings**](docs/Api/DepartmentApi.md#deletedepartmentworkinprogresssettings) | **DELETE** /organization/department/work-in-progress-settings | Delete the given department work in progress settings.
*DepartmentApi* | [**getDepartment**](docs/Api/DepartmentApi.md#getdepartment) | **GET** /organization/department/{department} | Returns a single department based on the given ID.
*DepartmentApi* | [**postDepartment**](docs/Api/DepartmentApi.md#postdepartment) | **POST** /organization/department | Create or update the department with the schema.
*EquipmentApi* | [**getEquipmentUnits**](docs/Api/EquipmentApi.md#getequipmentunits) | **GET** /equipment/units | Returns a list of equipment units associated with the organization.
*ExactOnlineApi* | [**getAccessibleDivisions**](docs/Api/ExactOnlineApi.md#getaccessibledivisions) | **GET** /exact-online/divisions | 
*HourLogApi* | [**getHourLogs**](docs/Api/HourLogApi.md#gethourlogs) | **GET** /project/{project}/hour-logs | Returns a list of hour logs associated with the given project.
*HourLogApi* | [**listContactHourLogs**](docs/Api/HourLogApi.md#listcontacthourlogs) | **GET** /list/hour-logs/contact | Returns a list of contact hour logs associated with your organization.
*HourLogApi* | [**listEmployeeHourLogs**](docs/Api/HourLogApi.md#listemployeehourlogs) | **GET** /list/hour-logs/employee | Returns a list of employee hour logs associated with your organization.
*I18nApi* | [**getCountries**](docs/Api/I18nApi.md#getcountries) | **GET** /i18n/countries | Returns all supported countries in the default locale if $locale parameter is not given.
*I18nApi* | [**getCurrencies**](docs/Api/I18nApi.md#getcurrencies) | **GET** /i18n/currencies | Returns all supported currencies in the default locale if $locale parameter is not given.
*I18nApi* | [**getLocales**](docs/Api/I18nApi.md#getlocales) | **GET** /i18n/locales | Returns all supported locales in the default locale if $locale parameter is not given.
*I18nApi* | [**getTimezones**](docs/Api/I18nApi.md#gettimezones) | **GET** /i18n/timezones | Returns all supported timezones in the default locale if $locale parameter is not given.
*InvoicingApi* | [**deleteInvoice**](docs/Api/InvoicingApi.md#deleteinvoice) | **DELETE** /invoice/{invoice} | Delete the given invoice.
*InvoicingApi* | [**getCollectiveInvoicePdf**](docs/Api/InvoicingApi.md#getcollectiveinvoicepdf) | **GET** /invoice/{invoice}/collective-pdf | Returns the PDF of an invoice by the given ID.
*InvoicingApi* | [**getInvoice**](docs/Api/InvoicingApi.md#getinvoice) | **GET** /invoice/{invoice} | Returns the document of an existing invoice.
*InvoicingApi* | [**getInvoiceCompanyInfo**](docs/Api/InvoicingApi.md#getinvoicecompanyinfo) | **GET** /invoicing-project/{project}/company-info | Returns the company information based on the given project.
*InvoicingApi* | [**getInvoiceEquipmentListPdf**](docs/Api/InvoicingApi.md#getinvoiceequipmentlistpdf) | **GET** /invoice/{invoice}/pdf/equipment-list | Returns the equipment list PDF of an invoice by the given ID.
*InvoicingApi* | [**getInvoiceGarbageListPdf**](docs/Api/InvoicingApi.md#getinvoicegarbagelistpdf) | **GET** /invoice/{invoice}/pdf/garbage-list | Returns the waste list PDF of an invoice by the given ID.
*InvoicingApi* | [**getInvoiceMailStatuses**](docs/Api/InvoicingApi.md#getinvoicemailstatuses) | **GET** /invoice/mail-statuses | Returns available statuses for an invoice mail.
*InvoicingApi* | [**getInvoiceMaterialListPdf**](docs/Api/InvoicingApi.md#getinvoicemateriallistpdf) | **GET** /invoice/{invoice}/pdf/material-list | Returns the material list of an invoice by the given ID.
*InvoicingApi* | [**getInvoicePdf**](docs/Api/InvoicingApi.md#getinvoicepdf) | **GET** /invoice/{invoice}/pdf | Returns the PDF of an invoice by the given ID.
*InvoicingApi* | [**listInvoices**](docs/Api/InvoicingApi.md#listinvoices) | **GET** /list/invoices | Returns a list of invoices associated with the organization.
*InvoicingApi* | [**makeAttachments**](docs/Api/InvoicingApi.md#makeattachments) | **POST** /invoice/{invoice}/make-attachments | Generate the given attachments for the given invoice.
*InvoicingApi* | [**newInvoice**](docs/Api/InvoicingApi.md#newinvoice) | **GET** /invoice/new | Returns the document of a new invoice.
*InvoicingApi* | [**newInvoiceForProject**](docs/Api/InvoicingApi.md#newinvoiceforproject) | **GET** /project/{project}/invoice/new | Returns the document of a new invoice.
*InvoicingApi* | [**updateInvoice**](docs/Api/InvoicingApi.md#updateinvoice) | **POST** /invoice | Creates or updates an invoice based on the given document.
*MileageRegistrationsApi* | [**deleteMileageRegistration**](docs/Api/MileageRegistrationsApi.md#deletemileageregistration) | **DELETE** /mileage-registration | Delete the given mileage registration.
*MileageRegistrationsApi* | [**getMileageRegistration**](docs/Api/MileageRegistrationsApi.md#getmileageregistration) | **GET** /mileage-registration/{id} | Returns a single mileage registration based on the given ID.
*MileageRegistrationsApi* | [**listMileageRegistrations**](docs/Api/MileageRegistrationsApi.md#listmileageregistrations) | **GET** /list/mileage-registrations | Returns a list of mileage registrations associated with your organization.
*MileageRegistrationsApi* | [**postMileageRegistration**](docs/Api/MileageRegistrationsApi.md#postmileageregistration) | **POST** /mileage-registration | Create or update the mileage registration with the schema.
*MobileSettingsApi* | [**deleteGlobalSetting**](docs/Api/MobileSettingsApi.md#deleteglobalsetting) | **DELETE** /mobile-settings/global | 
*MobileSettingsApi* | [**getGlobalSettings**](docs/Api/MobileSettingsApi.md#getglobalsettings) | **GET** /mobile-settings/global | 
*MobileSettingsApi* | [**getUserSettings**](docs/Api/MobileSettingsApi.md#getusersettings) | **GET** /mobile-settings | 
*MobileSettingsApi* | [**setGlobalSetting**](docs/Api/MobileSettingsApi.md#setglobalsetting) | **POST** /mobile-settings/global | 
*MobileSettingsApi* | [**setUserSetting**](docs/Api/MobileSettingsApi.md#setusersetting) | **POST** /mobile-settings | 
*OrganizationApi* | [**deleteCustomAttribute**](docs/Api/OrganizationApi.md#deletecustomattribute) | **DELETE** /organization/custom-attribute | Delete the given custom attribute.
*OrganizationApi* | [**deleteEmployee**](docs/Api/OrganizationApi.md#deleteemployee) | **DELETE** /organization/employee | Delete the given employee.
*OrganizationApi* | [**deleteHourType**](docs/Api/OrganizationApi.md#deletehourtype) | **DELETE** /organization/hour-type/{id} | Delete the given hour type.
*OrganizationApi* | [**deleteProjectCategory**](docs/Api/OrganizationApi.md#deleteprojectcategory) | **DELETE** /organization/project-category/{id} | Delete the given project category.
*OrganizationApi* | [**deleteProjectFileCategory**](docs/Api/OrganizationApi.md#deleteprojectfilecategory) | **DELETE** /organization/project-file-category/{id} | Delete the given project file category.
*OrganizationApi* | [**deleteQuotationStatus**](docs/Api/OrganizationApi.md#deletequotationstatus) | **DELETE** /organization/quotation-status/{id} | 
*OrganizationApi* | [**deleteTextTemplate**](docs/Api/OrganizationApi.md#deletetexttemplate) | **DELETE** /organization/text-template | Delete a text template.
*OrganizationApi* | [**getAllowedAccessTypes**](docs/Api/OrganizationApi.md#getallowedaccesstypes) | **GET** /organization/me/allowed-access-types | Returns a list of types that the currently authenticated user has access to.
*OrganizationApi* | [**getBasicEmployee**](docs/Api/OrganizationApi.md#getbasicemployee) | **GET** /organization/employee/basic/{id} | Returns basic data for a single employee based on the given ID.
*OrganizationApi* | [**getBranch**](docs/Api/OrganizationApi.md#getbranch) | **GET** /organization/branch/{id} | Returns a single branch based on the given ID.
*OrganizationApi* | [**getCurrentUser**](docs/Api/OrganizationApi.md#getcurrentuser) | **GET** /organization/me | Returns the user that is currently authenticated.
*OrganizationApi* | [**getCurrentUserPermissions**](docs/Api/OrganizationApi.md#getcurrentuserpermissions) | **GET** /organization/me/permissions | Returns the permissions for the currently authenticated user.
*OrganizationApi* | [**getCustomAttribute**](docs/Api/OrganizationApi.md#getcustomattribute) | **GET** /organization/custom-attribute/{id} | Returns a single custom attribute based on the given ID.
*OrganizationApi* | [**getDefaultProjectStatus**](docs/Api/OrganizationApi.md#getdefaultprojectstatus) | **GET** /organization/default-project-status | Return a list of default project statuses associated with your organization.
*OrganizationApi* | [**getDivision**](docs/Api/OrganizationApi.md#getdivision) | **GET** /organization/division/{id} | 
*OrganizationApi* | [**getEmployee**](docs/Api/OrganizationApi.md#getemployee) | **GET** /organization/employee/{id} | Returns a single employee based on the given ID.
*OrganizationApi* | [**getGeneralLedgerAccounts**](docs/Api/OrganizationApi.md#getgeneralledgeraccounts) | **GET** /organization/general-ledger-accounts | Return a list of general ledger accounts associated with your organization.
*OrganizationApi* | [**getHourType**](docs/Api/OrganizationApi.md#gethourtype) | **GET** /organization/hour-type/{id} | Returns a single hour type based on the given ID.
*OrganizationApi* | [**getHourTypes**](docs/Api/OrganizationApi.md#gethourtypes) | **GET** /organization/hour-types | Return hour types for the current authenticated user.
*OrganizationApi* | [**getOrganization**](docs/Api/OrganizationApi.md#getorganization) | **GET** /organization | Return basic information about the organization for the currently authenticated user.
*OrganizationApi* | [**getOrganizationHourTypePrices**](docs/Api/OrganizationApi.md#getorganizationhourtypeprices) | **GET** /organization/hour-type-prices | Returns all hour type prices associated with the organization.
*OrganizationApi* | [**getOrganizationSurchargePercentages**](docs/Api/OrganizationApi.md#getorganizationsurchargepercentages) | **GET** /organization/surcharge-percentages | Return a list of surcharge percentages associated with your organization.
*OrganizationApi* | [**getProjectCategories**](docs/Api/OrganizationApi.md#getprojectcategories) | **GET** /organization/project-categories | Return a set of project categories for the organization.
*OrganizationApi* | [**getProjectCategory**](docs/Api/OrganizationApi.md#getprojectcategory) | **GET** /organization/project-category/{id} | Returns a single project category based on the given ID.
*OrganizationApi* | [**getProjectFileCategories**](docs/Api/OrganizationApi.md#getprojectfilecategories) | **GET** /organization/project-file-categories | Returns a list of project file categories associated with your organization.
*OrganizationApi* | [**getProjectFileCategory**](docs/Api/OrganizationApi.md#getprojectfilecategory) | **GET** /organization/project-file-category/{id} | Returns a single project file category based on the given ID.
*OrganizationApi* | [**getQuotationStatus**](docs/Api/OrganizationApi.md#getquotationstatus) | **GET** /organization/quotation-status/{id} | Returns a single quotation status based on the given ID.
*OrganizationApi* | [**getTemplates**](docs/Api/OrganizationApi.md#gettemplates) | **GET** /organization/text-templates/{category} | 
*OrganizationApi* | [**getVatTariffs**](docs/Api/OrganizationApi.md#getvattariffs) | **GET** /organization/vat-tariffs | Return a set of VAT tariff objects that the organization can use, depending on the country.
*OrganizationApi* | [**listBasicEmployees**](docs/Api/OrganizationApi.md#listbasicemployees) | **GET** /list/basic-employees | Return a list of basic employee data associated with your organization.
*OrganizationApi* | [**listBranches**](docs/Api/OrganizationApi.md#listbranches) | **GET** /list/branches | Return a list of all branches associated with the organization.
*OrganizationApi* | [**listCommonInvoiceAttachments**](docs/Api/OrganizationApi.md#listcommoninvoiceattachments) | **GET** /list/common-invoice-attachments | Return a list of common invoice attachments associated with your organization.
*OrganizationApi* | [**listCommonQuotationAttachments**](docs/Api/OrganizationApi.md#listcommonquotationattachments) | **GET** /list/common-quotation-attachments | Return a list of common quotation attachments associated with your organization.
*OrganizationApi* | [**listCostCenters**](docs/Api/OrganizationApi.md#listcostcenters) | **GET** /list/cost-centers | Return a list of cost centers associated with your organization.
*OrganizationApi* | [**listCustomAttributes**](docs/Api/OrganizationApi.md#listcustomattributes) | **GET** /list/custom-attributes | Return a list of custom attributes for the organization.
*OrganizationApi* | [**listDepartments**](docs/Api/OrganizationApi.md#listdepartments) | **GET** /list/departments | Returns a list of departments associated with the organization.
*OrganizationApi* | [**listDivisions**](docs/Api/OrganizationApi.md#listdivisions) | **GET** /list/divisions | 
*OrganizationApi* | [**listEmployees**](docs/Api/OrganizationApi.md#listemployees) | **GET** /list/employees | Return a list of employees associated with your organization.
*OrganizationApi* | [**listProjectStatuses**](docs/Api/OrganizationApi.md#listprojectstatuses) | **GET** /list/project-statuses | Return a list of project statuses for the organization.
*OrganizationApi* | [**listQuotationConfirmationAttachments**](docs/Api/OrganizationApi.md#listquotationconfirmationattachments) | **GET** /list/quotation-confirmation-attachments | Return a list of quotation confirmation attachments associated with your organization.
*OrganizationApi* | [**listVatTariffs**](docs/Api/OrganizationApi.md#listvattariffs) | **GET** /list/vat-tariffs | Return a list of VAT tariff objects that the organization can use, depending on the country.
*OrganizationApi* | [**postBranch**](docs/Api/OrganizationApi.md#postbranch) | **POST** /organization/branch | Create or update the branch.
*OrganizationApi* | [**postCustomAttribute**](docs/Api/OrganizationApi.md#postcustomattribute) | **POST** /organization/custom-attributes | Create or update the custom attribute with the schema.
*OrganizationApi* | [**postEmployee**](docs/Api/OrganizationApi.md#postemployee) | **POST** /organization/employee | Create or update the employee.
*OrganizationApi* | [**postHourType**](docs/Api/OrganizationApi.md#posthourtype) | **POST** /organization/hour-type | Create or update the hour type.
*OrganizationApi* | [**postOrganizationHourTypePrice**](docs/Api/OrganizationApi.md#postorganizationhourtypeprice) | **POST** /organization/hour-type-price | Create or update the organization hour type price with the schema.
*OrganizationApi* | [**postProjectCategory**](docs/Api/OrganizationApi.md#postprojectcategory) | **POST** /organization/project-category | Create or update the project category.
*OrganizationApi* | [**postProjectFileCategory**](docs/Api/OrganizationApi.md#postprojectfilecategory) | **POST** /organization/project-file-category | Create or update the project file category.
*OrganizationApi* | [**postQuotationStatus**](docs/Api/OrganizationApi.md#postquotationstatus) | **POST** /organization/quotation-status | Create or update the quotation status.
*OrganizationApi* | [**postTextTemplate**](docs/Api/OrganizationApi.md#posttexttemplate) | **POST** /organization/text-template | Create or update a text template.
*ProjectApi* | [**canCreateInvoice**](docs/Api/ProjectApi.md#cancreateinvoice) | **GET** /project/{project}/invoicing/can-create | Returns true if an invoice can be made for the specified project.
*ProjectApi* | [**deleteInvoiceTermStatement**](docs/Api/ProjectApi.md#deleteinvoicetermstatement) | **DELETE** /project/term-statement | Delete the given project invoice term statement.
*ProjectApi* | [**deleteProject**](docs/Api/ProjectApi.md#deleteproject) | **DELETE** /project | Delete the given project.
*ProjectApi* | [**getDeletedProjects**](docs/Api/ProjectApi.md#getdeletedprojects) | **GET** /deleted-projects | Returns a list of deleted projects associated with the organization.
*ProjectApi* | [**getProject**](docs/Api/ProjectApi.md#getproject) | **GET** /project/{project} | Returns a project associated with the given id.
*ProjectApi* | [**getProjectFile**](docs/Api/ProjectApi.md#getprojectfile) | **GET** /project/file/{projectFile} | Returns a project file associated with the given id.
*ProjectApi* | [**hardDeleteProject**](docs/Api/ProjectApi.md#harddeleteproject) | **DELETE** /hard-delete-project/{projectId} | Deletes the given soft deleted project.
*ProjectApi* | [**listInvoiceTermStatements**](docs/Api/ProjectApi.md#listinvoicetermstatements) | **GET** /list/project-invoice-term-statements | Returns a list of project invoice term statements associated with the organization.
*ProjectApi* | [**listInvoiceTerms**](docs/Api/ProjectApi.md#listinvoiceterms) | **GET** /list/project-invoice-terms | Returns a list of project invoice terms associated with the organization.
*ProjectApi* | [**listProjects**](docs/Api/ProjectApi.md#listprojects) | **GET** /list/projects | Returns a list of projects associated with the organization.
*ProjectApi* | [**postInvoiceTermStatement**](docs/Api/ProjectApi.md#postinvoicetermstatement) | **POST** /project/{project}/invoice-term-statement | Create or update the given project invoice term statement.
*ProjectApi* | [**postProject**](docs/Api/ProjectApi.md#postproject) | **POST** /project | Creates or updates the given project.
*ProjectApi* | [**restoreProject**](docs/Api/ProjectApi.md#restoreproject) | **POST** /restore-project/{projectId} | Restores the given soft deleted project.
*ProjectApi* | [**setInternalNote**](docs/Api/ProjectApi.md#setinternalnote) | **POST** /project/set-internal-note | Sets the internal note of the given project.
*PropertyAssetApi* | [**deletePropertyAsset**](docs/Api/PropertyAssetApi.md#deletepropertyasset) | **DELETE** /property-asset | Removes the given property asset.
*PropertyAssetApi* | [**getPropertyAsset**](docs/Api/PropertyAssetApi.md#getpropertyasset) | **GET** /property-asset/{propertyAsset} | Returns a single property asset based on the given ID.
*PropertyAssetApi* | [**listPropertyAssets**](docs/Api/PropertyAssetApi.md#listpropertyassets) | **GET** /list/property-assets | Returns a list of property assets associated with the organization.
*PropertyAssetApi* | [**postPropertyAsset**](docs/Api/PropertyAssetApi.md#postpropertyasset) | **POST** /property-asset | Create or update a property asset with the data in the schema.
*PurchaseInvoicingApi* | [**deletePurchaseInvoice**](docs/Api/PurchaseInvoicingApi.md#deletepurchaseinvoice) | **DELETE** /purchase-invoice | Delete the given purchase invoice.
*PurchaseInvoicingApi* | [**getDefaultGeneralLedgerAccountCode**](docs/Api/PurchaseInvoicingApi.md#getdefaultgeneralledgeraccountcode) | **POST** /purchase-invoicing/default-general-ledger-account | Returns the default general ledger account based on the given contact id / branch id.
*PurchaseInvoicingApi* | [**getPurchaseInvoice**](docs/Api/PurchaseInvoicingApi.md#getpurchaseinvoice) | **GET** /purchase-invoicing/purchase-invoice/{id} | Returns a single purchase invoice based on the given ID.
*PurchaseInvoicingApi* | [**getPurchaseInvoiceStatuses**](docs/Api/PurchaseInvoicingApi.md#getpurchaseinvoicestatuses) | **GET** /purchase-invoicing/statuses | Returns available statuses for an purchase invoice.
*PurchaseInvoicingApi* | [**listPurchaseInvoices**](docs/Api/PurchaseInvoicingApi.md#listpurchaseinvoices) | **GET** /list/purchase-invoices | Returns a list of purchase invoices belonging to the organization.
*PurchaseInvoicingApi* | [**postPurchaseInvoice**](docs/Api/PurchaseInvoicingApi.md#postpurchaseinvoice) | **POST** /purchase-invoice | Create or update purchase invoice.
*PurchaseInvoicingApi* | [**updatePurchaseInvoiceStatus**](docs/Api/PurchaseInvoicingApi.md#updatepurchaseinvoicestatus) | **PUT** /purchase-invoice/{id}/update-status/{status} | Update the purchase invoice with the given status.
*QuotationApi* | [**deleteQuotationReminder**](docs/Api/QuotationApi.md#deletequotationreminder) | **DELETE** /quotation/reminder | Deletes a quotation reminder associated with the given ID.
*QuotationApi* | [**getQuotation**](docs/Api/QuotationApi.md#getquotation) | **GET** /quotation/{quotation} | Returns the document of an existing quotation.
*QuotationApi* | [**getQuotationReminder**](docs/Api/QuotationApi.md#getquotationreminder) | **GET** /quotation/reminder/{quotationReminder} | Returns a quotation reminder based on the given ID.
*QuotationApi* | [**listQuotationReminders**](docs/Api/QuotationApi.md#listquotationreminders) | **GET** /list/quotation-reminders | Returns a list of quotation reminders associated with your organization.
*QuotationApi* | [**listQuotationStatusLogs**](docs/Api/QuotationApi.md#listquotationstatuslogs) | **GET** /list/quotation-status-logs | Returns a list of quotation status logs associated with any quotation for your organization.
*QuotationApi* | [**listQuotations**](docs/Api/QuotationApi.md#listquotations) | **GET** /list/quotations | Returns a list of quotations associated with your organization.
*QuotationApi* | [**newQuotationForProject**](docs/Api/QuotationApi.md#newquotationforproject) | **GET** /quotation/{project}/new | Returns the document with the project information filled in for a new quotation.
*QuotationApi* | [**postQuotation**](docs/Api/QuotationApi.md#postquotation) | **POST** /quotation | Creates or updates an quotation based on the given document.
*QuotationApi* | [**postQuotationReminder**](docs/Api/QuotationApi.md#postquotationreminder) | **POST** /quotation/reminder | Create or update the quotation reminder.
*ResourceApi* | [**deleteEquipment**](docs/Api/ResourceApi.md#deleteequipment) | **DELETE** /equipment | Deletes an equipment item associated with the given id.
*ResourceApi* | [**deleteEquipmentBooking**](docs/Api/ResourceApi.md#deleteequipmentbooking) | **DELETE** /equipment-booking | Deletes an equipment booking associated with the given id.
*ResourceApi* | [**deleteEquipmentGroup**](docs/Api/ResourceApi.md#deleteequipmentgroup) | **DELETE** /equipment-group | Deletes an equipment group associated with the given id.
*ResourceApi* | [**deleteEquipmentUnit**](docs/Api/ResourceApi.md#deleteequipmentunit) | **DELETE** /equipment-unit/{id} | Deletes an equipment unit associated with the given ID.
*ResourceApi* | [**deleteMaterial**](docs/Api/ResourceApi.md#deletematerial) | **DELETE** /material/{material} | Deletes a material item associated with the given ID.
*ResourceApi* | [**deleteMaterialBooking**](docs/Api/ResourceApi.md#deletematerialbooking) | **DELETE** /material-booking | Deletes a material booking associated with the given ID.
*ResourceApi* | [**deleteMaterialPerUnit**](docs/Api/ResourceApi.md#deletematerialperunit) | **DELETE** /material-per-unit | Deletes the given material per unit.
*ResourceApi* | [**deleteMaterialUnit**](docs/Api/ResourceApi.md#deletematerialunit) | **DELETE** /material-unit/{id} | Deletes a material unit associated with the given ID.
*ResourceApi* | [**deleteResource**](docs/Api/ResourceApi.md#deleteresource) | **DELETE** /resource | Deletes a resource associated with the given id.
*ResourceApi* | [**deleteResourceBooking**](docs/Api/ResourceApi.md#deleteresourcebooking) | **DELETE** /resource-booking | Deletes a resource booking associated with the given id.
*ResourceApi* | [**deleteResourceGroup**](docs/Api/ResourceApi.md#deleteresourcegroup) | **DELETE** /resource-group | Deletes a resource group associated with the given id.
*ResourceApi* | [**deleteResourceUnit**](docs/Api/ResourceApi.md#deleteresourceunit) | **DELETE** /resource-unit | Deletes a resource unit associated with the given id.
*ResourceApi* | [**deleteWaste**](docs/Api/ResourceApi.md#deletewaste) | **DELETE** /waste/{id} | Deletes a waste item associated with the given id.
*ResourceApi* | [**deleteWasteBooking**](docs/Api/ResourceApi.md#deletewastebooking) | **DELETE** /waste-booking | Deletes a waste booking associated with the given ID.
*ResourceApi* | [**deleteWastePerUnit**](docs/Api/ResourceApi.md#deletewasteperunit) | **DELETE** /waste-per-unit | Deletes the given waste per unit.
*ResourceApi* | [**deleteWasteUnit**](docs/Api/ResourceApi.md#deletewasteunit) | **DELETE** /waste-unit/{wasteUnit} | Deletes a waste unit associated with the given ID.
*ResourceApi* | [**getEquipment**](docs/Api/ResourceApi.md#getequipment) | **GET** /equipment/{equipment} | Returns a single equipment item based on the given ID.
*ResourceApi* | [**getEquipmentBooking**](docs/Api/ResourceApi.md#getequipmentbooking) | **GET** /equipment-booking/{id} | Returns an equipment booking associated with the given id.
*ResourceApi* | [**getEquipmentGroup**](docs/Api/ResourceApi.md#getequipmentgroup) | **GET** /equipment-group/{id} | Returns an equipment group associated with the given id.
*ResourceApi* | [**getEquipmentGroups**](docs/Api/ResourceApi.md#getequipmentgroups) | **GET** /equipment-groups | Returns a list of equipment groups associated with the organization.
*ResourceApi* | [**getEquipmentUnit**](docs/Api/ResourceApi.md#getequipmentunit) | **GET** /equipment-unit/{equipmentUnit} | Returns a single equipment unit based on the given ID.
*ResourceApi* | [**getMaterial**](docs/Api/ResourceApi.md#getmaterial) | **GET** /material/{id} | Returns a single material based on the given ID.
*ResourceApi* | [**getMaterialPerUnit**](docs/Api/ResourceApi.md#getmaterialperunit) | **GET** /material-per-unit/{id} | Returns a single material per unit based on the given ID.
*ResourceApi* | [**getMaterialUnit**](docs/Api/ResourceApi.md#getmaterialunit) | **GET** /material-unit/{materialUnit} | Returns a single material unit based on the given ID.
*ResourceApi* | [**getResource**](docs/Api/ResourceApi.md#getresource) | **GET** /resource/{type}/{id} | Returns a resource associated with the given id.
*ResourceApi* | [**getResourceBooking**](docs/Api/ResourceApi.md#getresourcebooking) | **GET** /resource-booking/{type}/{id} | Returns a resource booking associated with the given id.
*ResourceApi* | [**getResourceBookings**](docs/Api/ResourceApi.md#getresourcebookings) | **GET** /resource-bookings/{type} | Returns a set of resource bookings by an organization, optionally filtered by project.
*ResourceApi* | [**getResourceGroup**](docs/Api/ResourceApi.md#getresourcegroup) | **GET** /resource-group/{type}/{id} | Returns an resource group associated with the given id.
*ResourceApi* | [**getResourceUnit**](docs/Api/ResourceApi.md#getresourceunit) | **GET** /resource-unit/{type}/{id} | Returns a resource unit associated with the given id.
*ResourceApi* | [**getResourceUnits**](docs/Api/ResourceApi.md#getresourceunits) | **GET** /resource-units/{type} | Returns a set of resource units associated with the organization.
*ResourceApi* | [**getResources**](docs/Api/ResourceApi.md#getresources) | **GET** /resources/{type} | Returns a set of resources associated with the organization.
*ResourceApi* | [**getWaste**](docs/Api/ResourceApi.md#getwaste) | **GET** /waste/{waste} | Returns a single waste item based on the given ID.
*ResourceApi* | [**getWasteBooking**](docs/Api/ResourceApi.md#getwastebooking) | **GET** /waste-booking/{wasteBooking} | Returns a waste booking associated with the given ID.
*ResourceApi* | [**getWastePerUnit**](docs/Api/ResourceApi.md#getwasteperunit) | **GET** /waste-per-unit/{id} | Returns a single waste per unit based on the given ID.
*ResourceApi* | [**getWasteUnit**](docs/Api/ResourceApi.md#getwasteunit) | **GET** /waste-unit/{id} | Returns a single waste unit based on the given ID.
*ResourceApi* | [**importMaterialPerUnits**](docs/Api/ResourceApi.md#importmaterialperunits) | **POST** /import/material-per-unit | Creates material records based on the given material per unit import list if the data is unique.
*ResourceApi* | [**importWastePerUnits**](docs/Api/ResourceApi.md#importwasteperunits) | **POST** /import/waste-per-unit | Creates waste records based on the given waste per unit import list if the data is unique.
*ResourceApi* | [**listEquipment**](docs/Api/ResourceApi.md#listequipment) | **GET** /list/equipment | Returns a list of equipment items owned by the organization.
*ResourceApi* | [**listEquipmentBookings**](docs/Api/ResourceApi.md#listequipmentbookings) | **GET** /list/booking/equipment | Returns a list of equipment bookings made by the organization.
*ResourceApi* | [**listEquipmentGroups**](docs/Api/ResourceApi.md#listequipmentgroups) | **GET** /list/equipment-groups | Returns a list of equipment groups owned by your organization.
*ResourceApi* | [**listEquipmentPerUnit**](docs/Api/ResourceApi.md#listequipmentperunit) | **GET** /list/equipment-per-unit | Returns a bookable list of units associated with a piece of equipment.
*ResourceApi* | [**listEquipmentUnits**](docs/Api/ResourceApi.md#listequipmentunits) | **GET** /list/equipment-units | Returns a list of equipment units owned by your organization.
*ResourceApi* | [**listGarbage**](docs/Api/ResourceApi.md#listgarbage) | **GET** /list/garbage | Returns a list of waste owned by the organization.
*ResourceApi* | [**listGarbageBookings**](docs/Api/ResourceApi.md#listgarbagebookings) | **GET** /list/booking/garbage | Returns a list of waste bookings made by the organization.
*ResourceApi* | [**listGarbagePerUnit**](docs/Api/ResourceApi.md#listgarbageperunit) | **GET** /list/garbage-per-unit | Returns a bookable list of units associated with waste.
*ResourceApi* | [**listMaterialBookings**](docs/Api/ResourceApi.md#listmaterialbookings) | **GET** /list/booking/material | Returns a list of material bookings made by the organization.
*ResourceApi* | [**listMaterialUnits**](docs/Api/ResourceApi.md#listmaterialunits) | **GET** /list/material-units | Returns a list of material units owned by your organization.
*ResourceApi* | [**listMaterials**](docs/Api/ResourceApi.md#listmaterials) | **GET** /list/materials | Returns a list of materials owned by your organization.
*ResourceApi* | [**listMaterialsPerUnit**](docs/Api/ResourceApi.md#listmaterialsperunit) | **GET** /list/materials-per-unit | Returns a bookable list of units associated with materials.
*ResourceApi* | [**listWaste**](docs/Api/ResourceApi.md#listwaste) | **GET** /list/waste | Returns a list of waste items owned by your organization.
*ResourceApi* | [**listWastePerUnit**](docs/Api/ResourceApi.md#listwasteperunit) | **GET** /list/waste-per-unit | Returns a bookable list of units associated with waste.
*ResourceApi* | [**listWasteUnits**](docs/Api/ResourceApi.md#listwasteunits) | **GET** /list/waste-units | Returns a list of waste units owned by your organization.
*ResourceApi* | [**postEquipment**](docs/Api/ResourceApi.md#postequipment) | **POST** /equipment | Create or update an equipment item.
*ResourceApi* | [**postEquipmentBooking**](docs/Api/ResourceApi.md#postequipmentbooking) | **POST** /equipment-booking | Create or update the equipment booking.
*ResourceApi* | [**postEquipmentGroup**](docs/Api/ResourceApi.md#postequipmentgroup) | **POST** /equipment-group | Creates or updates an equipment group for the currently authenticated user.
*ResourceApi* | [**postEquipmentUnit**](docs/Api/ResourceApi.md#postequipmentunit) | **POST** /equipment-unit | Create or update the equipment unit.
*ResourceApi* | [**postMaterial**](docs/Api/ResourceApi.md#postmaterial) | **POST** /material | Create or update the material.
*ResourceApi* | [**postMaterialPerUnit**](docs/Api/ResourceApi.md#postmaterialperunit) | **POST** /material-per-unit | Create or update the material per unit.
*ResourceApi* | [**postMaterialUnit**](docs/Api/ResourceApi.md#postmaterialunit) | **POST** /material-unit | Create or update the material unit.
*ResourceApi* | [**postResource**](docs/Api/ResourceApi.md#postresource) | **POST** /resource | Creates or updates a resource for the currently authenticated user.
*ResourceApi* | [**postResourceBooking**](docs/Api/ResourceApi.md#postresourcebooking) | **POST** /resource-booking | Creates or updates a resource booking for the currently authenticated user.
*ResourceApi* | [**postResourceGroup**](docs/Api/ResourceApi.md#postresourcegroup) | **POST** /resource-group | Creates or updates a resource group for the currently authenticated user.
*ResourceApi* | [**postResourceUnit**](docs/Api/ResourceApi.md#postresourceunit) | **POST** /resource-unit | Creates or updates a resource unit for the currently authenticated user.
*ResourceApi* | [**postWaste**](docs/Api/ResourceApi.md#postwaste) | **POST** /waste | Create or update a waste item.
*ResourceApi* | [**postWasteUnit**](docs/Api/ResourceApi.md#postwasteunit) | **POST** /waste-unit | Create or update the waste unit.
*SecurityApi* | [**getProjectSecurityLink**](docs/Api/SecurityApi.md#getprojectsecuritylink) | **GET** /project/project-security-link/{id} | Returns a single project security link based on the given ID.
*SecurityApi* | [**getSecurityObject**](docs/Api/SecurityApi.md#getsecurityobject) | **GET** /security-object/{id} | Returns a single security object based on the given ID.
*SecurityApi* | [**postSecurityObject**](docs/Api/SecurityApi.md#postsecurityobject) | **POST** /security-object | Create or update the security object.
*StorageApi* | [**deleteFile**](docs/Api/StorageApi.md#deletefile) | **DELETE** /storage/file | Deletes a file associated with the given id.
*StorageApi* | [**downloadFile**](docs/Api/StorageApi.md#downloadfile) | **GET** /storage/{hash}/download | Returns the binary or base64 contents of a file.
*StorageApi* | [**getFileContents**](docs/Api/StorageApi.md#getfilecontents) | **GET** /storage/{hash} | 
*StorageApi* | [**uploadFile**](docs/Api/StorageApi.md#uploadfile) | **POST** /storage/{modelType}/{modelId} | 
*UblApi* | [**generate**](docs/Api/UblApi.md#generate) | **GET** /ubl/generate/{invoice}/{version} | 
*UblApi* | [**getVersions**](docs/Api/UblApi.md#getversions) | **GET** /ubl/versions | 


## Documentation For Models

 - [AllowedAccessPerType](docs/Model/AllowedAccessPerType.md)
 - [Approval](docs/Model/Approval.md)
 - [ApprovalTemplateApprover](docs/Model/ApprovalTemplateApprover.md)
 - [ApprovalTemplateCriteria](docs/Model/ApprovalTemplateCriteria.md)
 - [ApprovalTemplateCriteriaList](docs/Model/ApprovalTemplateCriteriaList.md)
 - [ApprovalTemplateCriteriaListItem](docs/Model/ApprovalTemplateCriteriaListItem.md)
 - [ApprovalTemplateCriteriaRequirements](docs/Model/ApprovalTemplateCriteriaRequirements.md)
 - [ApprovalTemplateSettings](docs/Model/ApprovalTemplateSettings.md)
 - [ApprovalTemplateWorkflow](docs/Model/ApprovalTemplateWorkflow.md)
 - [ApprovalTemplateWorkflowList](docs/Model/ApprovalTemplateWorkflowList.md)
 - [ApprovalTemplateWorkflowListItem](docs/Model/ApprovalTemplateWorkflowListItem.md)
 - [ApprovalTemplateWorkflowSubType](docs/Model/ApprovalTemplateWorkflowSubType.md)
 - [ApprovalTemplateWorkflowTypes](docs/Model/ApprovalTemplateWorkflowTypes.md)
 - [ApprovalVote](docs/Model/ApprovalVote.md)
 - [AuditLog](docs/Model/AuditLog.md)
 - [BasicEmployee](docs/Model/BasicEmployee.md)
 - [BasicEmployeeList](docs/Model/BasicEmployeeList.md)
 - [BasicEmployeeListItem](docs/Model/BasicEmployeeListItem.md)
 - [BlameableUser](docs/Model/BlameableUser.md)
 - [BookingItemSummary](docs/Model/BookingItemSummary.md)
 - [BookingList](docs/Model/BookingList.md)
 - [BookingSummary](docs/Model/BookingSummary.md)
 - [Branch](docs/Model/Branch.md)
 - [BranchList](docs/Model/BranchList.md)
 - [BranchListItem](docs/Model/BranchListItem.md)
 - [CalledReceipt](docs/Model/CalledReceipt.md)
 - [CommonInvoiceAttachmentList](docs/Model/CommonInvoiceAttachmentList.md)
 - [CommonInvoiceAttachmentListItem](docs/Model/CommonInvoiceAttachmentListItem.md)
 - [CommonQuotationAttachment](docs/Model/CommonQuotationAttachment.md)
 - [CommonQuotationAttachmentList](docs/Model/CommonQuotationAttachmentList.md)
 - [CommonQuotationAttachmentListItem](docs/Model/CommonQuotationAttachmentListItem.md)
 - [CondensedApprovalTemplateCriteria](docs/Model/CondensedApprovalTemplateCriteria.md)
 - [CondensedApprovalTemplateWorkflow](docs/Model/CondensedApprovalTemplateWorkflow.md)
 - [CondensedApprover](docs/Model/CondensedApprover.md)
 - [CondensedBranch](docs/Model/CondensedBranch.md)
 - [CondensedContact](docs/Model/CondensedContact.md)
 - [CondensedContactPerson](docs/Model/CondensedContactPerson.md)
 - [CondensedContract](docs/Model/CondensedContract.md)
 - [CondensedContractOrderLine](docs/Model/CondensedContractOrderLine.md)
 - [CondensedCustomAttribute](docs/Model/CondensedCustomAttribute.md)
 - [CondensedCustomAttributeValue](docs/Model/CondensedCustomAttributeValue.md)
 - [CondensedDeliveryTicket](docs/Model/CondensedDeliveryTicket.md)
 - [CondensedDepartment](docs/Model/CondensedDepartment.md)
 - [CondensedDepartmentWipSettings](docs/Model/CondensedDepartmentWipSettings.md)
 - [CondensedDivision](docs/Model/CondensedDivision.md)
 - [CondensedEmployee](docs/Model/CondensedEmployee.md)
 - [CondensedEquipment](docs/Model/CondensedEquipment.md)
 - [CondensedEquipmentBooking](docs/Model/CondensedEquipmentBooking.md)
 - [CondensedEquipmentGroup](docs/Model/CondensedEquipmentGroup.md)
 - [CondensedEquipmentPerUnit](docs/Model/CondensedEquipmentPerUnit.md)
 - [CondensedEquipmentUnit](docs/Model/CondensedEquipmentUnit.md)
 - [CondensedFile](docs/Model/CondensedFile.md)
 - [CondensedHourType](docs/Model/CondensedHourType.md)
 - [CondensedInvoiceLine](docs/Model/CondensedInvoiceLine.md)
 - [CondensedInvoiceTermStatement](docs/Model/CondensedInvoiceTermStatement.md)
 - [CondensedMaterial](docs/Model/CondensedMaterial.md)
 - [CondensedMaterialBooking](docs/Model/CondensedMaterialBooking.md)
 - [CondensedMaterialPerUnit](docs/Model/CondensedMaterialPerUnit.md)
 - [CondensedMaterialUnit](docs/Model/CondensedMaterialUnit.md)
 - [CondensedProject](docs/Model/CondensedProject.md)
 - [CondensedProjectCategory](docs/Model/CondensedProjectCategory.md)
 - [CondensedProjectFileCategory](docs/Model/CondensedProjectFileCategory.md)
 - [CondensedProjectSecurityLink](docs/Model/CondensedProjectSecurityLink.md)
 - [CondensedProjectStatus](docs/Model/CondensedProjectStatus.md)
 - [CondensedPropertyAsset](docs/Model/CondensedPropertyAsset.md)
 - [CondensedPurchaseInvoice](docs/Model/CondensedPurchaseInvoice.md)
 - [CondensedPurchaseOrderContract](docs/Model/CondensedPurchaseOrderContract.md)
 - [CondensedQuotation](docs/Model/CondensedQuotation.md)
 - [CondensedQuotationReminder](docs/Model/CondensedQuotationReminder.md)
 - [CondensedQuotationStatus](docs/Model/CondensedQuotationStatus.md)
 - [CondensedResourceGroup](docs/Model/CondensedResourceGroup.md)
 - [CondensedSecurityCode](docs/Model/CondensedSecurityCode.md)
 - [CondensedSecurityObject](docs/Model/CondensedSecurityObject.md)
 - [CondensedSubcontractorContract](docs/Model/CondensedSubcontractorContract.md)
 - [CondensedTextTemplate](docs/Model/CondensedTextTemplate.md)
 - [CondensedUser](docs/Model/CondensedUser.md)
 - [CondensedVatTariff](docs/Model/CondensedVatTariff.md)
 - [CondensedWaste](docs/Model/CondensedWaste.md)
 - [CondensedWasteBooking](docs/Model/CondensedWasteBooking.md)
 - [CondensedWastePerUnit](docs/Model/CondensedWastePerUnit.md)
 - [CondensedWasteUnit](docs/Model/CondensedWasteUnit.md)
 - [ContactFinancialList](docs/Model/ContactFinancialList.md)
 - [ContactFinancialListItem](docs/Model/ContactFinancialListItem.md)
 - [ContactHourLogBooking](docs/Model/ContactHourLogBooking.md)
 - [ContactHourLogList](docs/Model/ContactHourLogList.md)
 - [ContactHourLogListItem](docs/Model/ContactHourLogListItem.md)
 - [ContactList](docs/Model/ContactList.md)
 - [ContactListItem](docs/Model/ContactListItem.md)
 - [ContactPerson](docs/Model/ContactPerson.md)
 - [ContactPersonList](docs/Model/ContactPersonList.md)
 - [ContactPersonListItem](docs/Model/ContactPersonListItem.md)
 - [ContactType](docs/Model/ContactType.md)
 - [ContractOrderLine](docs/Model/ContractOrderLine.md)
 - [ContractOrderLineList](docs/Model/ContractOrderLineList.md)
 - [ContractOrderLineListItem](docs/Model/ContractOrderLineListItem.md)
 - [ContractTerm](docs/Model/ContractTerm.md)
 - [CostCenterList](docs/Model/CostCenterList.md)
 - [CostCenterListItem](docs/Model/CostCenterListItem.md)
 - [CurrentUser](docs/Model/CurrentUser.md)
 - [CurrentUserEmployee](docs/Model/CurrentUserEmployee.md)
 - [CustomAttribute](docs/Model/CustomAttribute.md)
 - [CustomAttributeList](docs/Model/CustomAttributeList.md)
 - [CustomAttributeListItem](docs/Model/CustomAttributeListItem.md)
 - [DayOff](docs/Model/DayOff.md)
 - [DayOffList](docs/Model/DayOffList.md)
 - [DayOffListItem](docs/Model/DayOffListItem.md)
 - [DayOffPerEmployee](docs/Model/DayOffPerEmployee.md)
 - [DayOffPerEmployeeList](docs/Model/DayOffPerEmployeeList.md)
 - [DayOffPerEmployeeListItem](docs/Model/DayOffPerEmployeeListItem.md)
 - [DefaultPurchaseInvoiceSettingsFilter](docs/Model/DefaultPurchaseInvoiceSettingsFilter.md)
 - [DeletedProject](docs/Model/DeletedProject.md)
 - [DeliveryTicket](docs/Model/DeliveryTicket.md)
 - [DeliveryTicketBooking](docs/Model/DeliveryTicketBooking.md)
 - [DeliveryTicketList](docs/Model/DeliveryTicketList.md)
 - [DeliveryTicketListItem](docs/Model/DeliveryTicketListItem.md)
 - [DeliveryTicketWithProjectDetails](docs/Model/DeliveryTicketWithProjectDetails.md)
 - [Department](docs/Model/Department.md)
 - [DepartmentList](docs/Model/DepartmentList.md)
 - [DepartmentListItem](docs/Model/DepartmentListItem.md)
 - [DepartmentWipSettings](docs/Model/DepartmentWipSettings.md)
 - [Division](docs/Model/Division.md)
 - [DivisionBranchSettings](docs/Model/DivisionBranchSettings.md)
 - [DivisionBranchWipSettings](docs/Model/DivisionBranchWipSettings.md)
 - [DivisionList](docs/Model/DivisionList.md)
 - [DivisionListItem](docs/Model/DivisionListItem.md)
 - [DivisionProjectCategorySettings](docs/Model/DivisionProjectCategorySettings.md)
 - [DivisionWipSettings](docs/Model/DivisionWipSettings.md)
 - [Employee](docs/Model/Employee.md)
 - [EmployeeHourLogBooking](docs/Model/EmployeeHourLogBooking.md)
 - [EmployeeHourLogList](docs/Model/EmployeeHourLogList.md)
 - [EmployeeHourLogListItem](docs/Model/EmployeeHourLogListItem.md)
 - [EmployeeList](docs/Model/EmployeeList.md)
 - [EmployeeListItem](docs/Model/EmployeeListItem.md)
 - [Equipment](docs/Model/Equipment.md)
 - [EquipmentAttachmentType](docs/Model/EquipmentAttachmentType.md)
 - [EquipmentBooking](docs/Model/EquipmentBooking.md)
 - [EquipmentBooking2](docs/Model/EquipmentBooking2.md)
 - [EquipmentBookingList](docs/Model/EquipmentBookingList.md)
 - [EquipmentBookingListItem](docs/Model/EquipmentBookingListItem.md)
 - [EquipmentGroup](docs/Model/EquipmentGroup.md)
 - [EquipmentGroupList](docs/Model/EquipmentGroupList.md)
 - [EquipmentGroupListItem](docs/Model/EquipmentGroupListItem.md)
 - [EquipmentList](docs/Model/EquipmentList.md)
 - [EquipmentListItem](docs/Model/EquipmentListItem.md)
 - [EquipmentPerUnit](docs/Model/EquipmentPerUnit.md)
 - [EquipmentPerUnitList](docs/Model/EquipmentPerUnitList.md)
 - [EquipmentPerUnitListItem](docs/Model/EquipmentPerUnitListItem.md)
 - [EquipmentUnit](docs/Model/EquipmentUnit.md)
 - [EquipmentUnitList](docs/Model/EquipmentUnitList.md)
 - [EquipmentUnitListItem](docs/Model/EquipmentUnitListItem.md)
 - [File](docs/Model/File.md)
 - [FilteredHourLogCollection](docs/Model/FilteredHourLogCollection.md)
 - [FilteredResourceBookingCollection](docs/Model/FilteredResourceBookingCollection.md)
 - [FilteredResourceCollection](docs/Model/FilteredResourceCollection.md)
 - [FilteredResourceUnitCollection](docs/Model/FilteredResourceUnitCollection.md)
 - [FilteredVatTariffCollection](docs/Model/FilteredVatTariffCollection.md)
 - [FormFactor](docs/Model/FormFactor.md)
 - [FullContact](docs/Model/FullContact.md)
 - [FullContactDivision](docs/Model/FullContactDivision.md)
 - [GeneralLedgerAccount](docs/Model/GeneralLedgerAccount.md)
 - [GenerateAttachment](docs/Model/GenerateAttachment.md)
 - [HourLog](docs/Model/HourLog.md)
 - [HourLogBookingAttachmentType](docs/Model/HourLogBookingAttachmentType.md)
 - [HourType](docs/Model/HourType.md)
 - [HourTypePrice](docs/Model/HourTypePrice.md)
 - [HoursEstimatePerHourType](docs/Model/HoursEstimatePerHourType.md)
 - [InvoiceAttachment](docs/Model/InvoiceAttachment.md)
 - [InvoiceBranch](docs/Model/InvoiceBranch.md)
 - [InvoiceContact](docs/Model/InvoiceContact.md)
 - [InvoiceDocument](docs/Model/InvoiceDocument.md)
 - [InvoiceDocumentChapter](docs/Model/InvoiceDocumentChapter.md)
 - [InvoiceDocumentLine](docs/Model/InvoiceDocumentLine.md)
 - [InvoiceList](docs/Model/InvoiceList.md)
 - [InvoiceListItem](docs/Model/InvoiceListItem.md)
 - [InvoiceMail](docs/Model/InvoiceMail.md)
 - [InvoiceOrganization](docs/Model/InvoiceOrganization.md)
 - [InvoiceProject](docs/Model/InvoiceProject.md)
 - [InvoiceTermStatement](docs/Model/InvoiceTermStatement.md)
 - [LinkedBookingItem](docs/Model/LinkedBookingItem.md)
 - [Material](docs/Model/Material.md)
 - [MaterialAttachmentType](docs/Model/MaterialAttachmentType.md)
 - [MaterialBooking](docs/Model/MaterialBooking.md)
 - [MaterialBookingList](docs/Model/MaterialBookingList.md)
 - [MaterialBookingListItem](docs/Model/MaterialBookingListItem.md)
 - [MaterialGroup](docs/Model/MaterialGroup.md)
 - [MaterialList](docs/Model/MaterialList.md)
 - [MaterialListItem](docs/Model/MaterialListItem.md)
 - [MaterialPerDivision](docs/Model/MaterialPerDivision.md)
 - [MaterialPerUnit](docs/Model/MaterialPerUnit.md)
 - [MaterialPerUnitImport](docs/Model/MaterialPerUnitImport.md)
 - [MaterialPerUnitImportList](docs/Model/MaterialPerUnitImportList.md)
 - [MaterialPerUnitList](docs/Model/MaterialPerUnitList.md)
 - [MaterialPerUnitListItem](docs/Model/MaterialPerUnitListItem.md)
 - [MaterialUnit](docs/Model/MaterialUnit.md)
 - [MaterialUnitList](docs/Model/MaterialUnitList.md)
 - [MaterialUnitListItem](docs/Model/MaterialUnitListItem.md)
 - [MileageRegistration](docs/Model/MileageRegistration.md)
 - [MileageRegistrationList](docs/Model/MileageRegistrationList.md)
 - [MileageRegistrationListItem](docs/Model/MileageRegistrationListItem.md)
 - [MobileGlobalSetting](docs/Model/MobileGlobalSetting.md)
 - [MobileUserSetting](docs/Model/MobileUserSetting.md)
 - [ModulePermission](docs/Model/ModulePermission.md)
 - [NestedApprovalTemplateApproverListItem](docs/Model/NestedApprovalTemplateApproverListItem.md)
 - [NestedApprovalTemplateWorkflowListItem](docs/Model/NestedApprovalTemplateWorkflowListItem.md)
 - [NestedBranchListItem](docs/Model/NestedBranchListItem.md)
 - [NestedContactListItem](docs/Model/NestedContactListItem.md)
 - [NestedContactPersonListItem](docs/Model/NestedContactPersonListItem.md)
 - [NestedContactTypeListItem](docs/Model/NestedContactTypeListItem.md)
 - [NestedDeliveryTicketListItem](docs/Model/NestedDeliveryTicketListItem.md)
 - [NestedDepartmentListItem](docs/Model/NestedDepartmentListItem.md)
 - [NestedDivisionListItem](docs/Model/NestedDivisionListItem.md)
 - [NestedEmployeeListItem](docs/Model/NestedEmployeeListItem.md)
 - [NestedEquipmentGroupListItem](docs/Model/NestedEquipmentGroupListItem.md)
 - [NestedEquipmentListItem](docs/Model/NestedEquipmentListItem.md)
 - [NestedEquipmentPerUnitListItem](docs/Model/NestedEquipmentPerUnitListItem.md)
 - [NestedEquipmentUnitListItem](docs/Model/NestedEquipmentUnitListItem.md)
 - [NestedHourLogProjectListItem](docs/Model/NestedHourLogProjectListItem.md)
 - [NestedHourTypeListItem](docs/Model/NestedHourTypeListItem.md)
 - [NestedInvoiceLineListItem](docs/Model/NestedInvoiceLineListItem.md)
 - [NestedMaterialGroupListItem](docs/Model/NestedMaterialGroupListItem.md)
 - [NestedMaterialListItem](docs/Model/NestedMaterialListItem.md)
 - [NestedMaterialPerUnitListItem](docs/Model/NestedMaterialPerUnitListItem.md)
 - [NestedMaterialUnitListItem](docs/Model/NestedMaterialUnitListItem.md)
 - [NestedProjectCategoryListItem](docs/Model/NestedProjectCategoryListItem.md)
 - [NestedProjectInvoiceTermStatementListItem](docs/Model/NestedProjectInvoiceTermStatementListItem.md)
 - [NestedProjectListItem](docs/Model/NestedProjectListItem.md)
 - [NestedProjectSecurityCodeLinkListItem](docs/Model/NestedProjectSecurityCodeLinkListItem.md)
 - [NestedProjectStatusListItem](docs/Model/NestedProjectStatusListItem.md)
 - [NestedPropertyAssetListItem](docs/Model/NestedPropertyAssetListItem.md)
 - [NestedQuotationListItem](docs/Model/NestedQuotationListItem.md)
 - [NestedQuotationStatusListItem](docs/Model/NestedQuotationStatusListItem.md)
 - [NestedUserLinkListItem](docs/Model/NestedUserLinkListItem.md)
 - [NestedUserListItem](docs/Model/NestedUserListItem.md)
 - [NestedVatTariffListItem](docs/Model/NestedVatTariffListItem.md)
 - [NestedWasteListItem](docs/Model/NestedWasteListItem.md)
 - [NestedWastePerUnitListItem](docs/Model/NestedWastePerUnitListItem.md)
 - [NestedWasteUnitListItem](docs/Model/NestedWasteUnitListItem.md)
 - [Organization](docs/Model/Organization.md)
 - [PendingApprovalList](docs/Model/PendingApprovalList.md)
 - [PendingApprovalListItem](docs/Model/PendingApprovalListItem.md)
 - [Project](docs/Model/Project.md)
 - [ProjectCategory](docs/Model/ProjectCategory.md)
 - [ProjectFile](docs/Model/ProjectFile.md)
 - [ProjectFileCategory](docs/Model/ProjectFileCategory.md)
 - [ProjectFileMetadata](docs/Model/ProjectFileMetadata.md)
 - [ProjectInvoiceTerm](docs/Model/ProjectInvoiceTerm.md)
 - [ProjectInvoiceTermList](docs/Model/ProjectInvoiceTermList.md)
 - [ProjectInvoiceTermListItem](docs/Model/ProjectInvoiceTermListItem.md)
 - [ProjectInvoiceTermStatementListItem](docs/Model/ProjectInvoiceTermStatementListItem.md)
 - [ProjectList](docs/Model/ProjectList.md)
 - [ProjectListItem](docs/Model/ProjectListItem.md)
 - [ProjectSecurityLink](docs/Model/ProjectSecurityLink.md)
 - [ProjectSecurityLinkHourInfo](docs/Model/ProjectSecurityLinkHourInfo.md)
 - [ProjectStatus](docs/Model/ProjectStatus.md)
 - [ProjectStatusList](docs/Model/ProjectStatusList.md)
 - [ProjectStatusListItem](docs/Model/ProjectStatusListItem.md)
 - [PropertyAsset](docs/Model/PropertyAsset.md)
 - [PropertyAssetList](docs/Model/PropertyAssetList.md)
 - [PropertyAssetListItem](docs/Model/PropertyAssetListItem.md)
 - [PurchaseInvoiceDocument](docs/Model/PurchaseInvoiceDocument.md)
 - [PurchaseInvoiceDocumentLine](docs/Model/PurchaseInvoiceDocumentLine.md)
 - [PurchaseInvoiceLineBooking](docs/Model/PurchaseInvoiceLineBooking.md)
 - [PurchaseInvoiceList](docs/Model/PurchaseInvoiceList.md)
 - [PurchaseInvoiceListItem](docs/Model/PurchaseInvoiceListItem.md)
 - [PurchaseOrderContract](docs/Model/PurchaseOrderContract.md)
 - [PurchaseOrderContractHistory](docs/Model/PurchaseOrderContractHistory.md)
 - [PurchaseOrderContractList](docs/Model/PurchaseOrderContractList.md)
 - [PurchaseOrderContractListItem](docs/Model/PurchaseOrderContractListItem.md)
 - [PurchaseOrderContractTermList](docs/Model/PurchaseOrderContractTermList.md)
 - [PurchaseOrderContractTermListItem](docs/Model/PurchaseOrderContractTermListItem.md)
 - [Quotation](docs/Model/Quotation.md)
 - [QuotationAttachment](docs/Model/QuotationAttachment.md)
 - [QuotationConfirmationAttachmentList](docs/Model/QuotationConfirmationAttachmentList.md)
 - [QuotationConfirmationAttachmentListItem](docs/Model/QuotationConfirmationAttachmentListItem.md)
 - [QuotationLine](docs/Model/QuotationLine.md)
 - [QuotationLineChapter](docs/Model/QuotationLineChapter.md)
 - [QuotationList](docs/Model/QuotationList.md)
 - [QuotationListItem](docs/Model/QuotationListItem.md)
 - [QuotationMail](docs/Model/QuotationMail.md)
 - [QuotationReminder](docs/Model/QuotationReminder.md)
 - [QuotationReminderList](docs/Model/QuotationReminderList.md)
 - [QuotationReminderListItem](docs/Model/QuotationReminderListItem.md)
 - [QuotationStatus](docs/Model/QuotationStatus.md)
 - [QuotationStatusLogList](docs/Model/QuotationStatusLogList.md)
 - [QuotationStatusLogListItem](docs/Model/QuotationStatusLogListItem.md)
 - [Resource](docs/Model/Resource.md)
 - [ResourceBooking](docs/Model/ResourceBooking.md)
 - [ResourceBookingInfo](docs/Model/ResourceBookingInfo.md)
 - [ResourceBookingProjectInfo](docs/Model/ResourceBookingProjectInfo.md)
 - [ResourceEmployee](docs/Model/ResourceEmployee.md)
 - [ResourceGroup](docs/Model/ResourceGroup.md)
 - [ResourceGroupBookingInfo](docs/Model/ResourceGroupBookingInfo.md)
 - [ResourcePerUnit](docs/Model/ResourcePerUnit.md)
 - [ResourceProjectSecurityLink](docs/Model/ResourceProjectSecurityLink.md)
 - [ResourceUnit](docs/Model/ResourceUnit.md)
 - [ResourceUnitBookingInfo](docs/Model/ResourceUnitBookingInfo.md)
 - [SecurityObject](docs/Model/SecurityObject.md)
 - [SubcontractorContract](docs/Model/SubcontractorContract.md)
 - [SubcontractorContractHistory](docs/Model/SubcontractorContractHistory.md)
 - [SubcontractorContractList](docs/Model/SubcontractorContractList.md)
 - [SubcontractorContractListItem](docs/Model/SubcontractorContractListItem.md)
 - [SubcontractorContractTermList](docs/Model/SubcontractorContractTermList.md)
 - [SubcontractorContractTermListItem](docs/Model/SubcontractorContractTermListItem.md)
 - [SurchargeCollection](docs/Model/SurchargeCollection.md)
 - [Surcharges](docs/Model/Surcharges.md)
 - [TextTemplate](docs/Model/TextTemplate.md)
 - [UblVersions](docs/Model/UblVersions.md)
 - [UpdateInternalNote](docs/Model/UpdateInternalNote.md)
 - [VatTariff](docs/Model/VatTariff.md)
 - [VatTariffList](docs/Model/VatTariffList.md)
 - [VatTariffListItem](docs/Model/VatTariffListItem.md)
 - [Waste](docs/Model/Waste.md)
 - [WasteAttachmentType](docs/Model/WasteAttachmentType.md)
 - [WasteBooking](docs/Model/WasteBooking.md)
 - [WasteBooking2](docs/Model/WasteBooking2.md)
 - [WasteBookingList](docs/Model/WasteBookingList.md)
 - [WasteBookingListItem](docs/Model/WasteBookingListItem.md)
 - [WasteList](docs/Model/WasteList.md)
 - [WasteListItem](docs/Model/WasteListItem.md)
 - [WastePerUnit](docs/Model/WastePerUnit.md)
 - [WastePerUnitImport](docs/Model/WastePerUnitImport.md)
 - [WastePerUnitImportList](docs/Model/WastePerUnitImportList.md)
 - [WastePerUnitList](docs/Model/WastePerUnitList.md)
 - [WastePerUnitListItem](docs/Model/WastePerUnitListItem.md)
 - [WasteUnit](docs/Model/WasteUnit.md)
 - [WasteUnitList](docs/Model/WasteUnitList.md)
 - [WasteUnitListItem](docs/Model/WasteUnitListItem.md)


## Documentation For Authorization


## Bearer

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


## Author




