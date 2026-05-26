# Operationalizing Network & SErvice abstractioNs (ONSEN) WG Charter

Large networks rely on service abstraction mechanisms — for example, VPNs, service function chains, traffic engineering, attachment circuits, and network slicing — to deliver differentiated services and simplify provisioning. As the [IAB NEMOPS workshop](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/) highlighted, operational workflows for deploying, monitoring, and evolving these abstractions are inconsistent and poorly integrated, despite much of the underlying IETF prior work.

The ONSEN WG aims to make IETF service and network abstractions easier to implement and use, improving automation, operational efficiency, and interoperability. 

For this WG, the term "abstraction" refers to the process of defining simplified, constructs that represent network and service-level capabilities. Abstraction enables interaction between managed components and automation management systems without directly exposing the underlying device-specific implementations. The layer between the managed components and automation management system is referred to as "abstraction layer".

ONSEN will serve as the IETF's focal point for service and network abstraction modeling, with these core activities:

1. Documenting the use-cases, scope and priorities for network and service abstractions for work items identified in the charter.
1. Defining the abstraction layer, using device-level YANG models as the basis for the abstraction. As part of that, new service or network level YANG models will be developed as needed.
1. Updating key YANG data models, including refactoring or restructuring, which includes at least the following: VPN Common Model, L2VPN Service Model (L2SM), L3VPN Service Model (L3SM), L2VPN Network Model (L2NM), L3VPN Network Model (L3NM), Attachment Circuit Common Model, Attachment Circuit-as-a-Service (ACaaS), Attachment Circuit Network Model, Service Attachment Points (SAP), Network Slicing, Service Assurance for Intent-Based Networking (SAIN), Virtual Network (VN), Abstraction and Control of TE Networks (ACTN), and the YANG Data Model for Network and VPN Service Performance Monitoring.

Beyond these, ONSEN will produce informational documents describing service-layer APIs based on YANG service models for interfacing with OSS/BSS systems, enabling automated and interoperable service orchestration across systems and vendors. This includes guidance on mapping IETF YANG data models to external frameworks (e.g., TMF640) and on interfacing with external systems (e.g., network source of truth, IP address management). ONSEN will not normatively define or extend those external frameworks.

## Work Items

1. Develop a problem statement to define the use-cases, scope and priorities for the work items already identified in the charter. This should be taken from existing models, operator input, and the [IAB NEMOPS Workshop Report](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/).
1. Assess and update the YANG data models identified in the core activities
1. Develop service and network level YANG data models for the abstraction layer
1. Define the interface between YANG-based service APIs and the OSS/BSS layer

The WG may decide that some documents, such as the problem statement, use-cases, scope and priorities, are not intended for RFC publication and will be maintained as WG documents. The intended status of the remaining documents is Proposed Standard.

## Relationship With Existing WGs

* Technology or protocol-specific modeling efforts (e.g., device-level YANG data models) remain the responsibility of their respective WGs.
* ONSEN WG will engage with other relevant WGs (e.g., NETMOD and NMOP) to gather requirements and input related to tooling.
* Any new requirements for changes to the YANG language that are identified during ONSEN WG discussions will be directed to the NETMOD WG for consideration.
* BESS/CCAMP/TEAS: ONSEN WG will take on future network and service data modeling efforts, while technology or protocol-specific modeling efforts remain in these WGs.
* NMOP: ONSEN WG will focus on abstractions, while topology-related efforts will remain in NMOP. Network topology models are out of scope of ONSEN.
* OPSAWG: ONSEN WG will handle AC/SAP/L2NM/L3NM work going forward, enabling OPSAWG to focus on other operational topics. Future abstraction-related work will be directed to ONSEN.
* BESS/CCAMP/TEAS: Any network or service level modeling effort already adopted by these WG will remain in these WGs. However, ONSEN WG will take on future network and service data modeling efforts from these WGs.

## Milestones

| Date           | Milestone | Description | Intended Track |
|----------------|-----------|-------------|:--------------:|
| June 2026      | Send LSes to TMF, 3GPP, BBF, GSMA, Linux Foundation, TIP, and EANTC about ONSEN | Actively seek collaboration with other organizations | N/A |
| November 2026  | WG adoption of a problem statement draft defining the use-cases, scope and priorities for the work items identified in the WG, with input from operators and the [IAB NEMOPS Workshop Report](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/) | Draft providing a problem statement to define use-cases, scope and priorities for the current set of ONSEN activities | Not published as RFC |
| March 2027     | WG adoption of draft updating the YANG network data models for L3NM and L2NM | Updated drafts for L2NM and L3NM YANG data models based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| March 2027     | WG adoption of draft that updates the YANG service data models for L3SM and L2SM | Updated drafts for L3SM and L2SM YANG data models based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| June 2027      | WG adoption of draft updating the VPN Common Model | Updated draft for the VPN Common YANG data model based on operational feedback and deployment experiences | PS |
| July 2027      | WG adoption of a draft for Service-layer APIs based on YANG service models to interface with OSS/BSS | Draft detailing the Service-layer APIs based on YANG service models to interface with OSS/BSS | PS |
| July 2027      | WG adoption of a draft for new service and network level YANG data models for the abstraction layer | Draft detailing service and network level YANG data models | PS |
| July 2027      | WG adoption of draft updating the Network Slicing YANG data model | Updated draft for the Network Slicing YANG data model based on operational feedback and deployment experiences | PS |
| November 2027  | WG adoption of draft that updates the YANG data model for the Attachment Circuit Common Model | Updated draft for AC Common YANG data model based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| November 2027  | WG adoption of draft that updates the YANG data model for Attachment Circuit as a Service (ACaaS) | Updated draft for ACaaS YANG data model based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| November 2027  | WG adoption of draft updating the YANG data model for Service Assurance for Intent-Based Networking (SAIN) | Updated draft for the SAIN YANG data model based on operational feedback and deployment experiences | PS |
| November 2027  | WG adoption of draft updating the Virtual Network (VN) YANG data model | Updated draft for the VN YANG data model based on operational feedback and deployment experiences | PS |
| March 2028     | WG adoption of draft that updates the YANG data model for the Attachment Circuit Network Model | Updated draft for AC Network YANG data model based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| March 2028     | WG adoption of draft that updates the YANG data model for Service Attachment Points (SAP) | Updated draft for SAP YANG data model based on operational feedback and deployment experiences, with attention to operational state data and identified gaps | PS |
| March 2028     | WG adoption of draft updating the Abstraction and Control of TE Networks (ACTN) YANG data model | Updated draft for the ACTN YANG data model based on operational feedback and deployment experiences | PS |
| March 2028     | WG adoption of draft updating the YANG Data Model for Network and VPN Service Performance Monitoring | Updated draft for the Performance Monitoring YANG data model based on operational feedback and deployment experiences | PS |


