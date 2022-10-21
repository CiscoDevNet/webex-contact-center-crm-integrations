# Webex Contact Center CRM Integrations - Desktop Layouts - Freshdesk

Welcome to the Webex Contact Center CRM Integrations Github repository!

This folder contains the latest Desktop Layout for Freshdesk integrated Agent Desktop inside of the CRM console.

## Desktop Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

Administrators are free to customize the layout based on the description and functionality below.

| #   | Layout Properties | Description                                                                       | Functionality                                                                            |
| --- | ----------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| 1   | outdialAni        | This property allows you to override the Outdial ANI specified, for click to dial | Optional field. The default Outdial ANI set on the tenant or Agent Profile will be used. |
| 2   | crmLibPath        | Do not change                                                                     | Mandatory field.                                                                         |

## Desktop URLs per Datacenter

> Please note the Webex Contact Center Desktop URLs per Datacenter

| #   | Desktop URL                         | Data Center   |
| --- | ----------------------------------- | ------------- |
| 1   | https://desktop.wxcc-us1.cisco.com  | North America |
| 2   | https://desktop.wxcc-eu1.cisco.com  | UK            |
| 3   | https://desktop.wxcc-eu2.cisco.com  | EU            |
| 4   | https://desktop.wxcc-anz1.cisco.com | APJC          |

# Change Log :

The following change log shows the version updates to the files and what changes and enhacements were included:

(Please use the latest Desktop Layout JSON in the folder)

| #   | Date       | Filename                                 | Desktop Version | Comments                                                                                |
| --- | ---------- | ---------------------------------------- | --------------- | --------------------------------------------------------------------------------------- |
| 1   | April 2022 | Freshdesk_Desktop_0.0.6_v1.json          | 0.0.6           | + initial commit                                                                        |
| 2   | June 2022  | Freshdesk_Desktop_0.0.6_v2.json          | 0.0.6           | + Add headerActions[""] to the desktop layout so the action headers will be suppressed. |
| 3   | June 2022  | Freshdesk_Desktop_0.0.6_v1.json          | 0.0.6           | - removed                                                                               |
| 4   | Sept 2022  | Freshdesk_Desktop_0.0.6_v4_20220616.json | 0.0.6           | new endpoint                                                                            |

## Feature Matrix

This section outlines the features available in the standard connector as well as customizations that can be enabled on the desktop layout.

| #   | Feature​                                                                         | Standard Connector |
| --- | -------------------------------------------------------------------------------- | ------------------ |
| 1   | Auto-login of Agents into Contact Center platform (SSO)​                         | ✔️                 |
| 2   | Call Controls embedded in CRM application                                        | ✔️                 |
| 3   | Screen-pop based on incoming call parameters (No Record Match)                   | ✔️                 |
| 4   | Screen-pop based on incoming call parameters (Single record match - ANI)​        | ✔️                 |
| 5   | Screen-pop based on incoming call parameters (Multiple record Match - ANI)​      | ✔️                 |
| 6   | Outbound Calling – Click to Call​                                                | ✔️                 |
| 7   | Outbound Support                                                                 | ✔️                 |
| 8   | Automatic call (activity) logging in CRM application                             | ✔️                 |
| 9   | IVR Data populated within CRM (Caller Entered Digits captured as CAD variables)​ | ✔️                 |

## Installation Guide

The installation guide is available at **[help.webex.com - Integrate WebexCC With FreshDesk](https://help.webex.com/en-us/article/nb8oxvy/Integrate-Webex-Contact-Center-with-Freshdesk)**

## Support

Need Help? **[Contact Cisco TAC](https://cisco.com/go/tac)** to open a case.

Participate in discussions OR ask for help on the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
