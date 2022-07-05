# Webex Contact Center CRM Integrations - Desktop Layouts - Salesforce

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains the latest Desktop Layout and call center definition file for Salesforce integrated Agent Desktop inside of the CRM console.

## Call Center Definition Properties

The following section describes the properties in the call center definition file and their utility in turning on certain features.

Administrators are free to customize the call center definition file based on the description and functionality below.

| #   | Call Center Properties                                      | Description                                                                                               | Functionality                                              |
| --- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| 1   | CTI Adapter URL                                             | Should be same as Agent Desktop URL (based on production data centers)                                    | Mandatory field. Check the next section for URL details.   |
| 2   | Use CTI API                                                 | Flag to enable / disable ???                                                                              | Mandatory field. The value should be either true or false. |
| 3   | Softphone Height                                            | This property is used to set the desktop connector height.                                                | Optional field. Default desktop height will be considered. |
| 4   | Softphone Width                                             | This property is used to set the desktop connector width.                                                 | Optional field. Default desktop width will be considered.  |
| 5   | Salesforce Compatibility Mode                               | Select the compatibility mode (Lightning / Classic)                                                       | Mandatory field.                                           |
| 6   | Whether advanced screenpop enabled                          | Flag to enable / disable advanced search (CAD variable based search)                                      | Mandatory field. The value should be either true or false. |
| 7   | Screenpop search parameter CAD variable name                | CAD variable name whose value is to be searched in the CRM                                                | Mandatory field for advanced search.                       |
| 8   | Whether outdial phone number prefix to be removed           | Enabling this flag removes the specified prefix from the outdial number                                   | Optional field.                                            |
| 9   | Phone number prefix to be removed                           | Prefix to be removed from outdial number                                                                  | Optional field.                                            |
| 10  | Salesforce Package Namespace                                | Use ??                                                                                                    | Mandatory field ???                                        |
| 11  | Whether the activity record auto refresh enabled            | Enabling this flag refreshes the activity records list automatically                                      | Optional field ????                                        |
| 12  | Whether custom field needs to be updated in activity record | By enabling this flag customer can add additional custom fields in activity records.                      | Optional field. By default it will be 'false'              |
| 13  | WebexCC Salesforce field mapping                            | Mapping between CAD variables and CRM objects should be provided to add custom fields in activity record. | Optional field.                                            |
| 12  | DateFormat used in Subject                                  | Preferred date time format                                                                                | Optional field.                                            |

## Desktop / CTI Adapter URLs per Datacenter

CTI adapter url in the call center definition file will vary based on different regions of Webex contact center production data centers. By default the CTI adapter url points to US1 data center.

> Please note the Desktop / CTI Adapter URLs per Datacenter

| #   | Desktop / CTI Adapter URL           | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

## Change Log

The following change log shows the version updates to the files and what changes and enhacements were included:

(Please use the latest Desktop Layout JSON in the folder)

| #   | Date       | Filename                         | Desktop Version | Change Description       |
| --- | ---------- | -------------------------------- | --------------- | ------------------------ |
| 1   | Jan 2022   | Salesforce_Desktop.json          | 0.0.2           | First draft              |
| 2   | April 2022 | Salesforce_Desktop_v1.1.json     | 0.0.2           | Minor changes            |
| 3   | April 2022 | Salesforce_Desktop_0.0.6_v1.json | 0.0.6           | Desktop (Product) update |
