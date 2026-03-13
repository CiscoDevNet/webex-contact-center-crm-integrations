# Microsoft Dynamics 365 - Webex Contact Center Legacy Connector

![CRM](https://img.shields.io/badge/CRM-Microsoft%20Dynamics%20365-0A66C2)
![Legacy Version 1](https://img.shields.io/badge/Webex%20CC-Legacy%20Version%201-orange)
[![Official Guide](https://img.shields.io/badge/help.webex.com-Official%20Guide-blue)](https://help.webex.com/en-us/article/aw26j2/Integrate-Webex-Contact-Center-with-Microsoft-Dynamics-365-(Version-1%E2%80%94Legacy))

Legacy Version 1 desktop layout assets for the Microsoft Dynamics 365 embedded Webex Contact Center Agent Desktop. This folder includes the current layout package and the companion IVR HTTP connector reference bundle.

> Latest desktop layout: [`MSDynamics_Desktop_0.1.0_v1.5.3.json`](./MSDynamics_Desktop_0.1.0_v1.5.3.json)
>
> Companion bundle: [msdynamics-ivr-http-connector](./msdynamics-ivr-http-connector/README.md)
>
> Official guide: [Integrate Webex Contact Center with Microsoft Dynamics 365 (Version 1-Legacy)](https://help.webex.com/en-us/article/aw26j2/Integrate-Webex-Contact-Center-with-Microsoft-Dynamics-365-(Version-1%E2%80%94Legacy))

## Quick Links

| Asset | Purpose |
| --- | --- |
| [`MSDynamics_Desktop_0.1.0_v1.5.3.json`](./MSDynamics_Desktop_0.1.0_v1.5.3.json) | Latest Microsoft Dynamics 365 desktop layout package |
| [IVR HTTP connector bundle](./msdynamics-ivr-http-connector/README.md) | Sample flow, Postman collection, screenshots, and connector notes |

## Configuration Notes

- Set `hostName` to your Microsoft Dynamics 365 instance URL.
- When `isAdvancedScreenpopEnabled` is enabled, the related entity and field properties must also be configured.
- CIF 2.0 support, case management, and the Actions Widget are controlled through optional layout properties in the latest package.

## Desktop URLs by Datacenter

| Desktop URL | Datacenter |
| --- | --- |
| `https://desktop.wxcc-us1.cisco.com` | North America |
| `https://desktop.wxcc-eu1.cisco.com` | UK |
| `https://desktop.wxcc-eu2.cisco.com` | EU |
| `https://desktop.wxcc-anz1.cisco.com` | APJC |

## Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

| #   | Layout Property                          | Description                                                                                                       | Functionality                                                                                                                                                                                                    |
| --- | ---------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outdialAni                               | Override the Outdial ANI specified for click to dial                                                             | Optional field. The default Outdial ANI set on the tenant or agent profile will be used.                                                                                                                        |
| 2   | desktopWidth                             | Set the desktop connector width                                                                                  | Optional field. Default desktop width will be used.                                                                                                                                                              |
| 3   | hostName                                 | Hostname of the Microsoft Dynamics instance, for example `"https://org91c3bc64.crm.dynamics.com/"`             | Mandatory field.                                                                                                                                                                                                 |
| 4   | isAdvancedScreenpopEnabled               | Enable or disable advanced search (CAD-variable based search)                                                    | Mandatory field. The value should be either `true` or `false`.                                                                                                                                                   |
| 5   | cadVariableName                          | CAD variable name whose value is searched in the CRM                                                             | Mandatory field for advanced search.                                                                                                                                                                             |
| 6   | crmEntityName                            | Entity type in Microsoft Dynamics, for example Contact, Account, or Case                                         | Mandatory field for advanced search.                                                                                                                                                                             |
| 7   | crmEntityFieldName                       | Field name of the entity in Microsoft Dynamics within which the records are searched                             | Mandatory field for advanced search. See this [vidcast](https://app.vidcast.io/share/b84fea07-d72d-4fd9-ad75-691045392f43) for how to locate entity field names in your tenant.                               |
| 8   | inboundANIPrefixToBeRemoved              | Enable or disable removal of prefix from ANI for inbound calls                                                   | Optional field. Default value is `false`.                                                                                                                                                                        |
| 9   | inboundANIPrefix                         | Prefix to remove from ANI for record match and screen pop in CRM for inbound calls                               | Mandatory field when prefix removal is enabled.                                                                                                                                                                  |
| 10  | phoneCallActivityRecordConfig            | JSON object                                                                                                      | Desktop layout property to enable or disable automatic display and creation of phone call activity records.                                                                                                      |
| 11  | channelIntegrationFrameWorkVersion2Enabled | Enable or disable Channel Integration Framework (CIF) 2.0 support for Customer Service Workspace                | Desktop layout property to enable or disable CIF 2.0.                                                                                                                                                            |
| 12  | isWidgetDisplayEnabled                   | Enable or disable the Actions Widget                                                                             | Optional field.                                                                                                                                                                                                  |
| 13  | createActivityRecordConfig               | Phone call activity record configuration                                                                         | Optional field.                                                                                                                                                                                                  |
| 14  | openContactFormWithPrefilledDataConfig   | New contact form configuration                                                                                   | Optional field.                                                                                                                                                                                                  |
| 15  | createCaseRecordConfig                   | Case management configuration                                                                                    | Optional field.                                                                                                                                                                                                  |
| 16  | actionsWidgetConfig                      | Actions Widget feature configuration                                                                             | Optional field.                                                                                                                                                                                                  |

## Feature Matrix

This section outlines the features available in the standard connector as well as customizations that can be enabled on the desktop layout.

| #   | Feature | Standard Connector |
| --- | --- | --- |
| 1   | Auto-login of agents into Contact Center platform (SSO) | ✔️ |
| 2   | Call controls embedded in CRM application | ✔️ |
| 3   | Screen pop based on incoming call parameters (no record match) | ✔️ |
| 4   | Screen pop based on incoming call parameters (single record match - ANI) | ✔️ |
| 5   | Screen pop based on incoming call parameters (multiple record match - ANI) | ✔️ |
| 6   | Advanced screen pop based on incoming call parameters (other params such as case management) | ✔️ |
| 7   | Outbound calling - click to call | ✔️ |
| 8   | Outbound support | ✔️ |
| 9   | Automatic call activity logging in CRM | ✔️ |
| 10  | IVR data populated within CRM (caller-entered digits captured as CAD variables) | ✔️ |
| 11  | Contact Center reporting within the CRM | ✔️ |
| 12  | Activity ownership transfer during call transfer | - |
| 13  | Screen pop and activity logging retention during consult transfer or conference | ✔️ |
| 14  | Actions Widget | ✔️ |

## Additional Resources

- [Microsoft Dynamics IVR HTTP connector README](./msdynamics-ivr-http-connector/README.md)
- [CRM Integrations lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)

## Support

- Open a case with [Cisco TAC](https://cisco.com/go/tac).
- Ask questions in the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
