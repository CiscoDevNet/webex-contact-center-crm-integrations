# Integrate Webex Contact Center with Microsoft Dynamics

This folder contains the latest Desktop Layout for the Microsoft Dynamics integrated Agent Desktop inside of the CRM.

## Desktop Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

Administrators are free to customize the layout based on the description and functionality below.

| #   | Layout Properties           | Description                                                                                                      | Functionality                                                                                                                                                                                                                           |
| --- | --------------------------- | ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outdialAni                  | This property allows you to override the Outdial ANI specified, for click to dial                                | Optional field. The default Outdial ANI set on the tenant or Agent Profile will be used.                                                                                                                                                |
| 2   | desktopWidth                | This property is used to set the desktop connector width.                                                        | Optional field. Default desktop width will be considered.                                                                                                                                                                               |
| 3   | hostName                    | Hostname of the MS Dynamics Instance (Example : "hostName":"https://org91c3bc64.crm.dynamics.com/")              | Mandatory field.                                                                                                                                                                                                                        |
| 4   | isAdvancedScreenpopEnabled  | Flag to enable / disable advanced search (CAD variable based search)                                             | Mandatory field. The value should be either true or false.                                                                                                                                                                              |
| 5   | cadVariableName             | CAD variable name whose value is to be searched in the CRM                                                       | Mandatory field for advanced search.                                                                                                                                                                                                    |
| 6   | crmEntityName               | Entity type in the MS Dynamics. Example - Contact / Account / Case                                               | Mandatory field for advanced search.                                                                                                                                                                                                    |
| 7   | crmEntityFieldName          | Field name of the particular entity (crmEntityName) in MS Dynamics - within which the records are to be searched | Mandatory field for advanced search. Check [this](https://golive.anywhere365.io/platform_elements/webagent_for_dynamics365/scenarios/webagent_for_dynamcis365_cif_actions.html) for all the entity types and its associated field names |
| 8   | inboundANIPrefixToBeRemoved | Flag to enable / disable removal of prefix from ANI for Inbound Calls.                                           | Optional field. Default value will be false.                                                                                                                                                                                            |
| 9   | inboundANIPrefix            | Prefix to be removed from ANI for record match and screenpop in CRM for Inbound Calls. (Example : " "+1")        | Mandatory field for prefix removal.                                                                                                                                                                                                     |

## Desktop URLs per Datacenter

> Please note the Webex Contact Center Desktop URLs per Datacenter

| #   | Desktop URL                         | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

## Change Log

The following change log shows the version updates to the files and what changes and enhacements were included:

(Please use the latest Desktop Layout JSON in the folder)

| #   | File name                        | Desktop version | Change Description                                                                        | Change Date |
| --- | -------------------------------- | --------------- | ----------------------------------------------------------------------------------------- | ----------- |
| 1   | MSDynamics_Desktop.json          | 0.0.2           | First draft                                                                               | June 2021   |
| 2   | MSDynamics_Desktop_v1.1.json     | 0.0.2           | Minor changes                                                                             | August 2021 |
| 3   | MSDynamics_Desktop_0.0.6_v1.json | 0.0.6           | Desktop (Product) update                                                                  | April 2022  |
| 4   | MSDynamics_Desktop_0.0.6_v2.json | 0.0.6           | New feature - Advanced Screenpop / CAD variable based search                              | June 2022   |
| 5   | MSDynamics_Desktop_0.0.6_v3.json | 0.0.6           | New feature - Flag added to enable / disable removal of prefix from ANI for Inbound Calls | Aug 2022    |

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

## Installation Guide

The installation guide is available at **[help.webex.com](https://help.webex.com/en-us/article/aw26j2/Integrate-Webex-Contact-Center-with-Microsoft-Dynamics-365)**

## Lab Guides

Explore the **[CRM Integrations Lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)** that covers some of these integrations along with step by step instructions on the installation.

## Support

Need Help? **[Contact Cisco TAC](https://cisco.com/go/tac)** to open a case.

Participate in discussions OR ask for help on the [Cisco Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/5926-discussions-contact-center).
