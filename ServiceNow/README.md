# Webex Contact Center CRM Integrations - Desktop Layouts - ServiceNow

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains Desktop Layouts for the ServiceNow integrated Agent Desktop inside of the CRM console.

## Desktop Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

Administrators are free to customize the layout based on the description and functionality below.

| #   | Layout Properties                       | Description                                                                       | Functionality                                                                                                                                                                                                                |
| --- | --------------------------------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outDialAni                              | This property allows you to override the Outdial ANI specified, for click to dial | Optional field. The default Outdial ANI set on the tenant or Agent Profile will be used.                                                                                                                                     |
| 2   | screenpopCadName           | CAD variable name that has the value to be searched in CRM                        | Mandatory field for advanced search. If no value is provided, screenpop will be based on ANI search.                                                                                                                         |
| 3   | cadToCrmFieldMapping             | CAD variable name that can be stored in CRM logs. Ex: CadName1:SnowField1,CadName2:SnowField2   | Optional field.                                                                                                                                                                                         |
| 4   | crmLibPath                          | No change is required                                                        | Mandatory field. |

## Desktop URLs per Datacenter

> Please note the Webex Contact Center Desktop URLs per Datacenter

| #   | Desktop URL                         | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

## Change Log

The following change log shows the version updates to the file and what changes / enhacements were included:

(Please use the latest Desktop Layout JSON in the folder)

| #   | Date       | Filename                         | Version | Comments                                                                                                 |
| --- | ---------- | -------------------------------- | ------- | -------------------------------------------------------------------------------------------------------- |
| 1   | April 2022 | ServiceNow_Desktop_0.0.6_v1.json | 0.0.6   | + complete file                                                                                          |
| 2   | April 2022 | servicenow-update-setV3.xml      | V3      | + only used on dev instances - this file is not required for Enterprise licensed versions of Service Now |
| 3   | Sep 2022 | ServiceNow_Desktop_0.0.6_v2.0.0.json |v2.0.0   | + complete file                                                                                          |
| 4   | Sep 2022 |  webexcc-servicenow-update-setV4.xml | V4      | + only used on dev instances - this file is not required for Enterprise licensed versions of Service Now |
| 5   | Sep 2022 | ServiceNow_Desktop_0.0.6_v3.0.0.json |v3.0.0   | + complete file                                                                                          |
| 6   | Sep 2022 |  webexcc-servicenow-update-setv5.xml | v5      | + only used on dev instances - this file is not required for Enterprise licensed versions of Service Now |
