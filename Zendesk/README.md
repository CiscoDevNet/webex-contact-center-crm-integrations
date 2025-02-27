# Webex Contact Center CRM Integrations - Desktop Layouts - Zendesk

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains the latest Desktop Layout for Zendesk integrated Agent Desktop inside of the CRM console.

## Desktop Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

Administrators are free to customize the layout based on the description and functionality below.

| #   | Layout Properties                         | Description                                                                                                                                                                                                                                                          | Functionality                                                                                                                                                                                                                |
| --- | ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outdialAni                                | This property allows you to override the Outdial ANI specified, for click to dial                                                                                                                                                                                    | Optional field. The default Outdial ANI set on the tenant or Agent Profile will be used.                                                                                                                                     |
| 2   | isCaseCreationForAllInboundCallsEnabled   | Flag to enable / disable auto case creation for Inbound calls                                                                                                                                                                                                        | Mandatory field. The value should be either true or false.                                                                                                                                                                   |
| 3   | adavanceSearchCadVariableName             | CAD variable name that has the value to be searched in CRM                                                                                                                                                                                                           | Mandatory field for advanced search. If no value is provided, screenpop will be based on ANI search.                                                                                                                         |
| 4   | adavanceSearchCrmObjectName               | crm_object is the standard or custom Zendesk object like user, ticket etc. whereas crm_object_field is the standard or custom field of the Zendesk object like 'phone' field in the user object e.g. user npi : , where user = crm_object and npi = crm_object_field | Mandatory field for advanced search.                                                                                                                                                                                         |
| 5   | ticketDynamicField                        | Ticket field name                                                                                                                                                                                                                                                    | Optional field.                                                                                                                                                                                                              |
| 6   | ticketDynamicFieldValue                   | Ticket field value                                                                                                                                                                                                                                                   | Optional field.                                                                                                                                                                                                              |
| 7   | ticketDynamicSubject                      | Ticket dynamic Subject line                                                                                                                                                                                                                                          | Mandatory field. Define your own subject line (static or dynamic). Call parameters can be used for making the subject line dynamic (Example : {direction} call at {activityDateTime} -> Inbound call at 06.29.2022 12:01 p ) |
| 8   | dateTimeFormat                            | Preferred date time format                                                                                                                                                                                                                                           | Optional field - Default value will be used (MM.dd.yyyy hh:mm a)                                                                                                                                                             |
| 9   | customFieldsToBeUpdatedForExistingTickets | Flag to enable/disable the updation of custom fields for existing tickets after call wrap-up.                                                                                                                                                                        | Optional field - By default, it is disabled.                                                                                                                                                                                 |
| 10  | ticketCustomFieldsMapping                 | Use this feature to map the WebexCC CAD variables and Zendesk CRM Custom field IDs to auto populate CAD variable values in ticket object’s Custom fields while creating or updating ticket.                                                                          | Optional field - By default, it is disabled.                                                                                                                                                                                 |

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

| #   | File name                         | Desktop version | Change Description                                                                              | Change Date |
| --- | --------------------------------- | --------------- | ----------------------------------------------------------------------------------------------- | ----------- |
| 1   | Zendesk_Desktop.json              | 0.0.2           | Initial Layout Upload                                                                           | Nov 2021    |
| 2   | Zendesk_Desktop_v1.1.json         | 0.0.2           | Features: Ticket custom field added                                                             | Jan 2022    |
| 3   | Zendesk_Desktop_0.0.6_v1.json     | 0.0.6           | Features: Desktop (Product) update                                                              | April 2022  |
| 4   | Zendesk_Desktop_0.0.6_v2.json     | 0.0.6           | Features: Popup user list on widget for multi record match & Dynamic subject field added        | May 2022    |
| 5   | Zendesk_Desktop_0.0.6_v8.json     | 0.0.6           | Fixes: Widget reload issue fixed                                                                | Aug 2022    |
| 6   | Zendesk_Desktop_0.0.6_v1.1.1.json | 0.0.6           | Fixes: Added defensive validation for the widget reload issue.                                  | Sep 2022    |
| 7   | Zendesk_Desktop_0.0.6_v1.1.2.json | 0.0.6           | Fixes: Removed usage of deprecated APIs.                                                        | Oct 2022    |
| 8   | Zendesk_Desktop_0.0.6_v1.1.2.json | 0.0.6           | Fixes: Removed standard values of properties from the layout.                                   | Nov 2022    |
| 9   | Zendesk_Desktop_0.0.6_v1.1.2.json | 0.0.6           | Fixes: Desktop reload issue hotfix396.                                                          | Nov 2022    |
| 10  | Zendesk_Desktop_0.0.6_v1.2.0.json | 0.0.6           | Features: New feature added for populating call information in Custom Fields in Zendesk ticket. | Jan 2023    |
| 11  | Zendesk_Desktop_0.0.6_v1.2.2.json | 0.0.6           | Features: New feature added for ticket management | Feb 2025    |

## Feature Matrix

This section outlines the features available in the standard connector as well as customizations that can be enabled on the desktop layout.

| #   | Feature​                                                                                    | Standard Connector |
| --- | ------------------------------------------------------------------------------------------- | ------------------ |
| 1   | Auto-login of Agents into Contact Center platform (SSO)​                                    | ✔️                 |
| 2   | Call Controls embedded in CRM application                                                   | ✔️                 |
| 3   | Screen-pop based on incoming call parameters (No Record Match)                              | ✔️                 |
| 4   | Screen-pop based on incoming call parameters (Single record match - ANI)​                   | ✔️                 |
| 5   | Screen-pop based on incoming call parameters (Multiple record Match - ANI)​                 | ✔️                 |
| 6   | Advanced Screen-pop based on incoming call parameters (Other Params e.g., Case management)​ | ✔️                 |
| 7   | Outbound Calling – Click to Call​                                                           | ✔️                 |
| 8   | Outbound Support                                                                            | ✔️                 |
| 9   | Automatic call (activity) logging in CRM application                                        | ✔️                 |
| 10  | IVR Data populated within CRM (Caller Entered Digits captured as CAD variables)​            | ✔️                 |
| 11  | Contact Center Reporting within the CRM​                                                    | ✔️                 |
| 12  | Activity ownership transfer during Call Transfer​                                           | -                  |
| 13  | Screen-pop and activity logging retention during consult transfer/conference​               | ✔️                 |
| 14  | Ticket management                                                                          | ✔️                 |

## Installation Guide

The installation guide is available at **[help.webex.com](https://help.webex.com/en-us/article/jg2krv/Integrate-Webex-Contact-Center-with-Zendesk)**

## Lab Guides

Explore the **[CRM Integrations Lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)** that covers some of these integrations along with step by step instructions on the installation.

## Support

Need Help? **[Contact Cisco TAC](https://cisco.com/go/tac)** to open a case.

Participate in discussions OR ask for help on the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
