# Webex Contact Center CRM Integrations - Desktop Layouts - Salesforce

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains the latest Desktop Layout and call center definition file for Salesforce integrated Agent Desktop inside of the CRM console.

The CTI adapter url for the call center definition file will vary based on different regions of Webex contact center production data centers. By default the CTI adapter url points to US1 data center. The CTI adapter url for different data centers are listed below:

> Please note the CTI Adapter URLs for different data centers:

| #   | CTI Adapter URL                     | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

## Change Log

The following change log shows the version updates to the files and what changes and enhacements were included:

(Please use the latest Desktop Layout JSON in the folder)

| #   | Date       | Filename                             | Desktop Version | Change Description       | Change Date |
| --- | ---------- | ------------------------------------ | --------------- | ------------------------ | ----------- |
| 1   | Jan 2022   | Salesforce_Desktop.json              | 0.0.2           | First draft              | June 2021   |
| 2   | April 2022 | Salesforce_Desktop_v1.1.json         | 0.0.2           | Minor changes            | Sep 2021    |
| 3   | April 2022 | Salesforce_Desktop_0.0.6_v1.json     | 0.0.6           | Desktop (Product) update | April 2022  |
| 4   | Sep 2022   | salesforce_desktop_0.0.6_v1.0.1.json | 0.0.6           | New feature sets         | Sept 2022   |

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
| 10  | IVR Data populated within Salesforce (Caller Entered Digits captured as CAD variables)​     | ✔️                 |
| 11  | Contact Center Reporting within the CRM​                                                    | ✔️                 |
| 12  | Activity ownership transfer during Call Transfer​                                           | ✔️                 |
| 13  | Screen-pop and activity logging retention during consult transfer/conference​               | ✔️                 |
| 14  | On demand country code removal from inbound call ANI field                                  | ✔️                 |
| 15  | Custom screenpop settings for no record match screenpop search                              | ✔️                 |
| 16  | Recording of call live notes update to activity record                                      | ✔️                 |
| 17  | Dynamic activity record subject                                                             | ✔️                 |
| 18  | Case management                                                                             | ✔️                 |
| 19  | Omni state sync                                                                             | ✔️                 |
| 20  | SFDC actions widget                                                                         | ✔️                 |

## Installation Guide

The installation guide is available at **[help.webex.com](https://help.webex.com/en-us/article/nhxw7kfb/Integrate-Webex-Contact-Center-with-Salesforce)**

## Lab Guides

Explore the **[CRM Integrations Lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)** that covers some of these integrations along with step by step instructions on the installation.

## Support

Need Help? **[Contact Cisco TAC](https://cisco.com/go/tac)** to open a case.

Participate in discussions OR ask for help on the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
