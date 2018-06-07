

# Billing API

API layer to club Billing calls via a simple and powerful API. 


## Resources

Documentation for various API resources can be found separately in the
following locations:
### we can put the WSDL Url's right here 
- [Broadcast Messages](broadcast_messages.md)
- [Project-level Variables](project_level_variables.md)
- [Deployments](deployments.md)



## Wave 1 API Inventory and Usage info

| ID | ID   | Service Name              | Operation Name           | Description                                                                                                             | Comments Prepaid      | Comments Postpaid                                             | MyBill SA       |
|----|------|---------------------------|--------------------------|-------------------------------------------------------------------------------------------------------------------------|-----------------------|---------------------------------------------------------------|--------------|
| 1  | 1.1  | AddressRoleService        | createAddressRole        | wsdl/AddressRole.wsdl         | Not ready for Prepaid | --2044                                                     | -- |
|    | 1.2  | AddressRoleService        | readAddressRole          |                                                                                                                         |                       |                                                               |              |
|    | 1.3  | AddressRoleService        | updateAddressRole        |                                                                                                                         |                       |                                                               |              |
|    | 1.4  | AddressRoleService        | deleteAddressRole        |                                                                                                                         |                       |                                                               |              |
| 2  | 2.1  | PaymentArrangementService | createPaymentArrangement | wsdl/PaymentArrangement.wsdl  | NA                    |                                                               |              |
|    | 2.2  | PaymentArrangementService | readPaymentArrangement   |                                                                                                                         |                       |                                                               | -- |
|    | 2.3  | PaymentArrangementService | updatePaymentArrangement |                                                                                                                         |                       |                                                               |              |
|    | 2.4  | PaymentArrangementService | deletePaymentArrangement |                                                                                                                         |                       |                                                               |              |
| 3  | 3.1  | PartyRoleService          | createPartyRole          | wsdl/PartyRole.wsdl           |                       |                                                               |              |
|    | 3.2  | PartyRoleService          | readPartyRole            |                                                                                                                         | NA                    | 1314 , integartion READ only                           | -- |
|    | 3.3  | PartyRoleService          | updatePartyRole          |                                                                                                                         |                       |                                                               |              |
|    | 3.4  | PartyRoleService          | deletePartyRole          |                                                                                                                         |                       |                                                               |              |
| 4  | 4.1  | PartyRelationshipService  | createPartyRelationship  | wsdl/PartyRelationship.wsdl   |                       |                                                               |              |
|    | 4.2  | PartyRelationshipService  | readPartyRelationship    |                                                                                                                         |                       |                                                               |              |
|    | 4.3  | PartyRelationshipService  | updatePartyRelationship  |                                                                                                                         |                       |                                                               |              |
|    | 4.4  | PartyRelationshipService  | deletePartyRelationship  |                                                                                                                         |                       |                                                               |              |
| 5  | 5.1  | Invoice                   | createInvoice            | wsdl/Invoice.wsdl             |                       |                                                               |              |
|    | 5.2  | Invoice                   | readInvoice              |                                                                                                                         | NA                    | --1446 , integrating READ only                         | -- |
|    | 5.3  | Invoice                   | updateInvoice            |                                                                                                                         |                       |                                                               |              |
|    | 5.4  | Invoice                   | deleteInvoice            |                                                                                                                         |                       |                                                               |              |
| 6  | 6.1  | FinancialAccountService   | createFinancialAccount   | wsdl/FinancialAccount.wsdl    |                       |                                                               |              |
|    | 6.2  | FinancialAccountService   | readFinancialAccount     |                                                                                                                         | NA                    | --1446 , integrating with FinancialAccount READ only    | -- |
|    | 6.3  | FinancialAccountService   | updateFinancialAccount   |                                                                                                                         |                       |                                                               |              |
|    | 6.4  | FinancialAccountService   | deleteFinancialAccount   |                                                                                                                         | NA                    | 1313 , Integartion with ProspectCustomerCreate (SCOPE) | -- |
| 7  | 7.1  | CustomerService           | createCustomer           | wsdl/Customer.wsdl            |                       |             |              |
|    | 7.2  | CustomerService           | readCustomer             |                                                                                                                         |                       | --2050                                                     |              |
|    | 7.3  | CustomerService           | updateCustomer           |                                                                                                                         |                       | --1194                                                     |              |
|    | 7.4  | CustomerService           | deleteCustomer           |                                                                                                                         |                       |                                                               |              |
|    | 7.5  | CustomerService           | searchCustomer           |                                                                                                                         |                       |                                                               |              |
| 8  | 8.1  | SessionPass               | createSessionPass        | wsdl/SessionPass.wsdl         |                       |                                                               |              |
|    | 8.2  | SessionPass               | readSessionPass          |                                                                                                                         |                       |                                                               |              |
|    | 8.3  | SessionPass               | updateSessionPass        |                                                                                                                         |                       |                                                               |              |
|    | 8.4  | SessionPass               | deleteSessionPass        |                                                                                                                         |                       |                                                               |              |
|    |      |                           |                          |                                                                                                                         |                       |                                                               |              |
| 9  | 9.1  | CommunicationMethod       | readCommunicationMethod  | wsdl/CommunicationMethod.wsdl |                       |                                                               |              |
|    |      | emailCommunication        | read                     |                                                                                                                         |                       |                                                               |              |
|    |      | phoneCommunication        | read                     |                                                                                                                         |                       |                                                               |              |
|    |      | address Communication     | read                     |                                                                                                                         |                       |                                                               |              |
|    |      |                           |                          |                                                                                                                         |                       |                                                               |              |
| 10 | 10.1 | CustomerStatusHistory     | read                     |                                                                                                                         |                       |                                                               |              |
|    |      |                           |                          |                                                                                                                         |                       |                                                               |              |
| 11 | 11.1 | NetworkRequest            | createNetworkRequest     | wsdl/NetworkRequest.wsdl      |                       | --2107                                                     |              |
|    | 11.2 | NetworkRequest            | readNetworkRequest       |                                                                                                                         |                       |                                                               |              |
|    | 11.3 | NetworkRequest            | updateNetworkRequest     |                                                                                                                         |                       |                                                               |              |
|    | 11.4 | NetworkRequest            | deleteNetworkRequest     |                                                                                                                         |                       |                                                               |              |



## Wave 2 API details

| ID | Service Name |	Operation Name	| Description | Comments Prepaid | Comments Postpaid | MyBill SA |
| -- | ------------ | ----------------- | ----------- | ---------------- | ----------------- | ------ |
| 1.1  | LineOfService |	createLineOfService |	wsdl/LineOfService.wsdl| NA for Prepaid | |	--|
| 1.2  | LineOfService |	readLineOfService |	| NA for Prepaid | |	--|
| 1.3  | LineOfService |	updateLineOfService |	| NA for Prepaid | |	--|
| 1.4  |LineOfService |	deleteLineOfService |	| NA for Prepaid | |	--|
| 2.1  | NetworkRequestService |	createNetworkRequest |	wsdl/NetworkRequest.wsdl| NA for Prepaid | |	--|


## MyBill REST API basics

The following table gives an overview of how the API functions generally behave.

| Request type | Description |
| ------------ | ----------- |
| `GET`   | Access one or more resources and return the result as JSON. |
| `POST`  | Return `201 Created` if the resource is successfully created and return the newly created resource as JSON. |
| `GET` / `PUT` | Return `200 OK` if the resource is accessed or modified successfully. The (modified) result is returned as JSON. |
| `DELETE` | Returns `204 No Content` if the resuource was deleted successfully. |
