# Freshdesk - Webex Contact Center Legacy Connector

![CRM](https://img.shields.io/badge/CRM-Freshdesk-2CA01C)
![Legacy Version 1](https://img.shields.io/badge/Webex%20CC-Legacy%20Version%201-orange)
[![Official Guide](https://img.shields.io/badge/help.webex.com-Official%20Guide-blue)](https://help.webex.com/en-us/article/nb8oxvy/Integrate-Webex-Contact-Center-with-Freshdesk)

Legacy Version 1 desktop layout assets for the Freshdesk embedded Webex Contact Center Agent Desktop. This folder contains the current layout package for the legacy connector.

> Latest desktop layout: [`Freshdesk_Desktop_0.1.0_2.1.4.json`](./Freshdesk_Desktop_0.1.0_2.1.4.json)
>
> Official guide: [Integrate Webex Contact Center with Freshdesk](https://help.webex.com/en-us/article/nb8oxvy/Integrate-Webex-Contact-Center-with-Freshdesk)

## Quick Links

| Asset | Purpose |
| --- | --- |
| [`Freshdesk_Desktop_0.1.0_2.1.4.json`](./Freshdesk_Desktop_0.1.0_2.1.4.json) | Latest Freshdesk desktop layout package |

## Configuration Notes

- `crmLibPath` is mandatory and should not be changed.
- `outdialAni` can be used to override the Outdial ANI for click-to-dial behavior.
- The current package includes the ticket group configuration updates added in the latest changelog entry.

## Desktop URLs by Datacenter

| Desktop URL | Datacenter |
| --- | --- |
| `https://desktop.wxcc-us1.cisco.com` | North America |
| `https://desktop.wxcc-eu1.cisco.com` | UK |
| `https://desktop.wxcc-eu2.cisco.com` | EU |
| `https://desktop.wxcc-anz1.cisco.com` | APJC |

## Layout Properties

The following section describes the properties in the layout and their utility in turning on certain features.

| #   | Layout Property | Description                                                                       | Functionality                                                                             |
| --- | --------------- | --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| 1   | outdialAni      | Override the Outdial ANI specified for click to dial                              | Optional field. The default Outdial ANI set on the tenant or agent profile will be used. |
| 2   | crmLibPath      | Do not change                                                                     | Mandatory field.                                                                          |

## Feature Matrix

This section outlines the features available in the standard connector as well as customizations that can be enabled on the desktop layout.

| #   | Feature | Standard Connector |
| --- | --- | --- |
| 1   | Auto-login of agents into Contact Center platform (SSO) | ✔️ |
| 2   | Call controls embedded in CRM application | ✔️ |
| 3   | Screen pop based on incoming call parameters (no record match) | ✔️ |
| 4   | Screen pop based on incoming call parameters (single record match - ANI) | ✔️ |
| 5   | Screen pop based on incoming call parameters (multiple record match - ANI) | ✔️ |
| 6   | Outbound calling - click to call | ✔️ |
| 7   | Outbound support | ✔️ |
| 8   | Automatic call activity logging in CRM | ✔️ |
| 9   | IVR data populated within CRM (caller-entered digits captured as CAD variables) | ✔️ |

## Support

- Open a case with [Cisco TAC](https://cisco.com/go/tac).
- Ask questions in the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
