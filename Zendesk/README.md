# Zendesk - Webex Contact Center Legacy Connector

![CRM](https://img.shields.io/badge/CRM-Zendesk-03363D)
![Legacy Version 1](https://img.shields.io/badge/Webex%20CC-Legacy%20Version%201-orange)
[![Official Guide](https://img.shields.io/badge/help.webex.com-Official%20Guide-blue)](https://help.webex.com/en-us/article/jg2krv/Integrate-Webex-Contact-Center-with-Zendesk)

Legacy Version 1 desktop layout assets for the Zendesk embedded Webex Contact Center Agent Desktop. This folder includes the current layout package and the companion IVR HTTP connector reference bundle.

> Latest desktop layout: [`Zendesk_Desktop_0.1.0_v1.2.2.json`](./Zendesk_Desktop_0.1.0_v1.2.2.json)
>
> Companion bundle: [zendesk-ivr-http-connector](./zendesk-ivr-http-connector/README.md)
>
> Official guide: [Integrate Webex Contact Center with Zendesk](https://help.webex.com/en-us/article/jg2krv/Integrate-Webex-Contact-Center-with-Zendesk)

## Quick Links

| Asset | Purpose |
| --- | --- |
| [`Zendesk_Desktop_0.1.0_v1.2.2.json`](./Zendesk_Desktop_0.1.0_v1.2.2.json) | Latest Zendesk desktop layout package |
| [IVR HTTP connector bundle](./zendesk-ivr-http-connector/README.md) | Sample flow, Postman collection, screenshots, and connector notes |

## Preview

![Zendesk preview](./zendesk-ivr-http-connector/images/MainFlow.png)

## Configuration Notes

- `adavanceSearchCadVariableName` and `adavanceSearchCrmObjectName` control the advanced search behavior used for screen pop.
- Ticket subject customization, custom field mapping, and ticket management are all enabled through layout properties in the package.
- The date and subject formatting behavior remains driven by the values configured in the layout JSON.

## Desktop URLs by Datacenter

| Desktop URL | Datacenter |
| --- | --- |
| `https://desktop.wxcc-us1.cisco.com` | North America |
| `https://desktop.wxcc-eu1.cisco.com` | UK |
| `https://desktop.wxcc-eu2.cisco.com` | EU |
| `https://desktop.wxcc-anz1.cisco.com` | APJC |

## Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

| #   | Layout Property                         | Description                                                                                                                                                                                                                                                          | Functionality                                                                                                                                                                                                                |
| --- | --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | outdialAni                              | Override the Outdial ANI specified for click to dial                                                                                                                                                                                                                 | Optional field. The default Outdial ANI set on the tenant or agent profile will be used.                                                                                                                                    |
| 2   | isCaseCreationForAllInboundCallsEnabled | Enable or disable auto case creation for inbound calls                                                                                                                                                                                                               | Mandatory field. The value should be either `true` or `false`.                                                                                                                                                              |
| 3   | adavanceSearchCadVariableName           | CAD variable name that has the value to be searched in CRM                                                                                                                                                                                                           | Mandatory field for advanced search. If no value is provided, screen pop is based on ANI search.                                                                                                                            |
| 4   | adavanceSearchCrmObjectName             | Standard or custom Zendesk object and field to search, for example `user.phone`                                                                                                                                                                                     | Mandatory field for advanced search.                                                                                                                                                                                         |
| 5   | ticketDynamicField                      | Ticket field name                                                                                                                                                                                                                                                    | Optional field.                                                                                                                                                                                                              |
| 6   | ticketDynamicFieldValue                 | Ticket field value                                                                                                                                                                                                                                                   | Optional field.                                                                                                                                                                                                              |
| 7   | ticketDynamicSubject                    | Ticket dynamic subject line                                                                                                                                                                                                                                          | Mandatory field. Define your own subject line. Call parameters can be used to make the subject line dynamic.                                                                                                                |
| 8   | dateTimeFormat                          | Preferred date and time format                                                                                                                                                                                                                                       | Optional field. Default value is `MM.dd.yyyy hh:mm a`.                                                                                                                                                                      |
| 9   | customFieldsToBeUpdatedForExistingTickets | Enable or disable updates to custom fields for existing tickets after call wrap-up                                                                                                                                                                                 | Optional field. Disabled by default.                                                                                                                                                                                         |
| 10  | ticketCustomFieldsMapping               | Map Webex Contact Center CAD variables to Zendesk custom field IDs                                                                                                                                                                                                  | Optional field. Disabled by default.                                                                                                                                                                                         |

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
| 14  | Ticket management | ✔️ |

## Additional Resources

- [Zendesk IVR HTTP connector README](./zendesk-ivr-http-connector/README.md)
- [CRM Integrations lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)

## Support

- Open a case with [Cisco TAC](https://cisco.com/go/tac).
- Ask questions in the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
