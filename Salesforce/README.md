# Salesforce - Webex Contact Center Legacy Connector

![CRM](https://img.shields.io/badge/CRM-Salesforce-00A1E0)
![Legacy Version 1](https://img.shields.io/badge/Webex%20CC-Legacy%20Version%201-orange)
[![Official Guide](https://img.shields.io/badge/help.webex.com-Official%20Guide-blue)](https://help.webex.com/en-us/article/nhxw7kfb/Integrate-Webex-Contact-Center-with-Salesforce-(Version-1%E2%80%94Legacy))

Legacy Version 1 desktop layout assets for the Salesforce embedded Webex Contact Center Agent Desktop experience. This folder includes the primary desktop layout package, the Salesforce call center definition file, and the companion IVR HTTP connector reference bundle.

> Latest desktop layout: [`salesforce_desktop_0.1.0_v1.1.9.json`](./salesforce_desktop_0.1.0_v1.1.9.json)
>
> Companion file: [`sfdc-callcenter-definition-file.xml`](./sfdc-callcenter-definition-file.xml)
>
> Official guide: [Integrate Webex Contact Center with Salesforce (Version 1-Legacy)](https://help.webex.com/en-us/article/nhxw7kfb/Integrate-Webex-Contact-Center-with-Salesforce-(Version-1%E2%80%94Legacy))

## Quick Links

| Asset | Purpose |
| --- | --- |
| [`salesforce_desktop_0.1.0_v1.1.9.json`](./salesforce_desktop_0.1.0_v1.1.9.json) | Latest Salesforce desktop layout package in this repository |
| [`sfdc-callcenter-definition-file.xml`](./sfdc-callcenter-definition-file.xml) | Salesforce call center definition file |
| [IVR HTTP connector bundle](./salesforce-ivr-http-connector/README.md) | Sample flow, Postman collection, screenshots, and connector notes |

## Configuration Notes

- The CTI adapter URL in the call center definition file varies by Webex Contact Center production datacenter.
- The shipped definition file points to the US1 desktop URL by default and must be updated if your tenant is hosted elsewhere.
- The nested IVR HTTP connector folder is kept for reference and troubleshooting but is out of scope for this README refresh.

## CTI Adapter URLs by Datacenter

| CTI Adapter URL | Datacenter |
| --- | --- |
| `https://desktop.wxcc-us1.cisco.com` | North America |
| `https://desktop.wxcc-eu1.cisco.com` | UK |
| `https://desktop.wxcc-eu2.cisco.com` | EU |
| `https://desktop.wxcc-anz1.cisco.com` | APJC |

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
| 10  | IVR data populated within Salesforce (caller-entered digits captured as CAD variables) | ✔️ |
| 11  | Contact Center reporting within the CRM | ✔️ |
| 12  | Activity ownership transfer during call transfer | ✔️ |
| 13  | Screen pop and activity logging retention during consult transfer or conference | ✔️ |
| 14  | Automatic phone call activity record opening in edit mode on connected or wrap-up state | ✔️ |
| 15  | On-demand country code removal from inbound ANI | ✔️ |
| 16  | Custom screen pop settings for no-record-match search | ✔️ |
| 17  | Recording of live notes updates to the activity record | ✔️ |
| 18  | Dynamic activity record subject | ✔️ |
| 19  | Case management | ✔️ |
| 20  | Omni state sync | ✔️ |
| 21  | SFDC Actions Widget | ✔️ |

## Additional Resources

- [Salesforce IVR HTTP connector README](./salesforce-ivr-http-connector/README.md)
- [CRM Integrations lab guide](https://wxcctechsummit.github.io/wxcclabguides/TechSummitRoW_2021/CRM.html)

## Support

- Open a case with [Cisco TAC](https://cisco.com/go/tac).
- Ask questions in the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
