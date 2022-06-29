# Webex Contact Center CRM Integrations - Desktop Layouts - Zendesk

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains the latest Desktop Layout for the Zendesk integrated Agent Desktop inside of the CRM console.

## Desktop Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

Administrators are free to customize the layout based on the description and functionality below.

| #   | Layout Properties                       | Description                                                                     | Functionality                                                                                                                                                                                                                |
| --- | --------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outdialAni                              | To override the Outdial ANI specified for click to dial                         | Optional. The default Outdial ANI set on the tenant or Agent Profile will be used.                                                                                                                                           |
| 2   | isCaseCreationForAllInboundCallsEnabled | Flag to enable / disable auto case creation for Inbound calls                   | Mandatory field. The value should be either true or false.                                                                                                                                                                   |
| 3   | adavanceSearchCadVariableName           | CAD variable name that has the value to be searched in CRM                      | Optional field. Default ANI based search will be done for screenpop.                                                                                                                                                         |
| 4   | adavanceSearchCrmObjectName             | CRM object name in Zendesk within which the CAD variable value will be searched | Optional field. Default ANI based search will be done for screenpop.                                                                                                                                                         |
| 5   | ticketDynamicField                      | Ticket field name                                                               | Optional field.                                                                                                                                                                                                              |
| 6   | ticketDynamicFieldValue                 | Ticket field value                                                              | Optional field.                                                                                                                                                                                                              |
| 7   | ticketDynamicSubject                    | Ticket dynamic Subject line                                                     | Mandatory field. Define your own subject line (static or dynamic). Call parameters can be used for making the subject line dynamic (Example : {direction} call at {activityDateTime} -> Inbound call at 06.29.2022 12:01 p ) |
| 8   | dateTimeFormat                          | Preferred date time format                                                      | Optional field - Default value will be used (MM.dd.yyyy hh:mm a)                                                                                                                                                             |

## Desktop URLs per Datacenter

> Please note the Webex Contact Center Desktop URLs per Datacenter

| #   | Desktop URL                         | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

# Change Log :

The following change log shows the version updates to the files, what changes and enhacements were included.
(Please use the latest Desktop Layout JSON in the folder)

| #   | File name                     | Desktop version | Comment         | Change Description                                           |
| --- | ----------------------------- | --------------- | --------------- | ------------------------------------------------------------ |
| 1   | Zendesk_Desktop.json          | 0.0.2           | - header        | First draft                                                  |
| 2   | Zendesk_Desktop_v1.1.json     | 0.0.2           | - headless      | New feature - Advanced Screenpop / CAD variable based search |
| 3   | Zendesk_Desktop_0.0.6_v1.json | 0.0.6           | + complete file | New feature - Ticket dynamic custom field added              |
| 4   | Zendesk_Desktop_0.0.6_v2.json | 0.0.6           | headless        | New feature - Ticket dynamic subject field added             |
