# Webex Contact Center CRM Integrations - Legacy Version 1

![License](https://img.shields.io/github/license/CiscoDevNet/webex-contact-center-crm-integrations)
![Last Commit](https://img.shields.io/github/last-commit/CiscoDevNet/webex-contact-center-crm-integrations)
![Legacy Version 1](https://img.shields.io/badge/Webex%20CC-Legacy%20Version%201-orange)
![Connectors](https://img.shields.io/badge/connectors-5-success)

Legacy Version 1 desktop layouts and companion assets for Webex Contact Center CRM integrations. This repository is the public landing point for the Salesforce, ServiceNow, Microsoft Dynamics 365, Zendesk, and Freshdesk connector packages referenced by the official help.webex.com guides.

## Supported Connectors

| Connector | Latest layout asset | Other included assets | Official guide |
| --- | --- | --- | --- |
| [Salesforce](./Salesforce/README.md) | [`salesforce_desktop_0.1.0_v1.1.9.json`](./Salesforce/salesforce_desktop_0.1.0_v1.1.9.json) | [`sfdc-callcenter-definition-file.xml`](./Salesforce/sfdc-callcenter-definition-file.xml), [IVR HTTP connector](./Salesforce/salesforce-ivr-http-connector/README.md) | [Salesforce - Legacy install guide](https://help.webex.com/en-us/article/nhxw7kfb/Integrate-Webex-Contact-Center-with-Salesforce-(Version-1%E2%80%94Legacy)) |
| [ServiceNow](./ServiceNow/README.md) | [`ServiceNow_Desktop_0.1.0_v4.0.1.json`](./ServiceNow/ServiceNow_Desktop_0.1.0_v4.0.1.json) | [`webexcc-servicenow-update-setv7-1.xml`](./ServiceNow/webexcc-servicenow-update-setv7-1.xml), [ActionsWidget bundle](./ServiceNow/ActionsWidget/), [IVR HTTP connector](./ServiceNow/servicenow-ivr-http-connector/README.md) | [ServiceNow - Legacy install guide](https://help.webex.com/en-us/article/54vvw/Integrate-Webex-Contact-Center-with-ServiceNow-(Version-1%E2%80%94Legacy)) |
| [Microsoft Dynamics 365](./MS%20Dynamics/README.md) | [`MSDynamics_Desktop_0.1.0_v1.5.3.json`](./MS%20Dynamics/MSDynamics_Desktop_0.1.0_v1.5.3.json) | [IVR HTTP connector](./MS%20Dynamics/msdynamics-ivr-http-connector/README.md) | [Microsoft Dynamics 365 - Legacy install guide](https://help.webex.com/en-us/article/aw26j2/Integrate-Webex-Contact-Center-with-Microsoft-Dynamics-365-(Version-1%E2%80%94Legacy)) |
| [Zendesk](./Zendesk/README.md) | [`Zendesk_Desktop_0.1.0_v1.2.2.json`](./Zendesk/Zendesk_Desktop_0.1.0_v1.2.2.json) | [IVR HTTP connector](./Zendesk/zendesk-ivr-http-connector/README.md) | [Zendesk - Legacy install guide](https://help.webex.com/en-us/article/jg2krv/Integrate-Webex-Contact-Center-with-Zendesk) |
| [Freshdesk](./Freshdesk/README.md) | [`Freshdesk_Desktop_0.1.0_2.1.4.json`](./Freshdesk/Freshdesk_Desktop_0.1.0_2.1.4.json) | Desktop layout package only | [Freshdesk - Legacy install guide](https://help.webex.com/en-us/article/nb8oxvy/Integrate-Webex-Contact-Center-with-Freshdesk) |

## What This Repo Contains

- Legacy Version 1 desktop layouts for the five supported CRM connectors.
- Companion files such as call center definitions, update sets, and HTTP connector examples.
- Connector-specific README files with setup context, datacenter URLs, feature summaries, and changelog history.
- Existing sample flows and screenshots that help operators understand the legacy integration behavior.

## How To Use This Repo

1. Open the connector README that matches your CRM platform.
2. Download the latest layout asset and any companion files listed for that connector.
3. Follow the linked help.webex.com installation guide for the full setup workflow.

## Repository Layout

```text
.
|-- Salesforce/
|-- ServiceNow/
|-- MS Dynamics/
|-- Zendesk/
`-- Freshdesk/
```

Each connector folder keeps the public README, the latest layout package, and any related legacy assets in one place.

## Support

- Open a support case with [Cisco TAC](https://cisco.com/go/tac).
- Ask implementation questions in the [Cisco Developer Community for Webex Contact Center](https://community.cisco.com/t5/contact-center/bd-p/j-disc-dev-contact-center).
- Use the help.webex.com guides linked above for the full step-by-step installation instructions.
