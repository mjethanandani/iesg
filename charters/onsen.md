# Operationalizing Network & SErvice abstractioNs (ONSEN) WG Charter

Large networks rely on service abstraction mechanisms — for example, VPNs, service function chains, traffic engineering, attachment circuits, and network slicing — to deliver differentiated services and simplify provisioning. As the [IAB NEMOPS workshop](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/) highlighted, operational workflows for deploying, monitoring, and evolving these abstractions are inconsistent and poorly integrated, despite much of the underlying IETF prior work.

The ONSEN WG aims to make IETF service and network abstractions easier to implement and use, improving automation, operational efficiency, and interoperability. 

For this WG, the term "abstraction" refers to the process of defining simplified, constructs that represent network and service-level capabilities. Abstraction enables interaction between managed components and automation management systems without directly exposing the underlying device-specific implementations.

ONSEN will serve as the IETF's focal point for service and network abstraction modeling, with these core activities:

1. Documenting the use-cases, scope and priorities for network and service abstractions for work items identified in the charter.
1. Defining the abstraction layer, using device-level YANG models as the basis for the abstraction. As part of that, new service or network level YANG models will be developed as needed.
1. Updating key YANG data models, including refactoring or restructuring, which includes at least the following: VPN Common Model, L2VPN Service Model (L2SM), L3VPN Service Model (L3SM), L2VPN Network Model (L2NM), L3VPN Network Model (L3NM), Attachment Circuit Common Model, Attachment Circuit-as-a-Service (ACaaS), Attachment Circuit Network Model, Service Attachment Points (SAP), Network Slicing, Service Assurance for Intent-Based Networking (SAIN), Virtual Network (VN), Abstraction and Control of TE Networks (ACTN), and the YANG Data Model for Network and VPN Service Performance Monitoring.

Beyond these, ONSEN will define service-layer APIs based on YANG service models to interface with OSS/BSS, enabling automated and interoperable service orchestration across systems and vendors. This includes defining mechanisms and approaches for integrating IETF YANG data models with external frameworks (e.g., TMF640) and external systems (e.g., network source of truth, IP address management). 

The WG will catalogue tooling resources (tools, gaps, recommendations, implementation examples, hackathon artifacts) in the WG GitHub and/or Wiki, and actively encourage participation in hackathons and interoperability events.

## Work Items

1. Develop a problem statement to define the use-cases, scope and priorities for the work items already identified in the charter. This should be taken from existing models, operator input, and the [IAB NEMOPS Workshop Report](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/).
1. Update the YANG network data models for L3NM and L2NM
1. Update the YANG service data models for L3SM and L2SM
1. Develop service and network level YANG data models for the abstraction layer
1. Define the interface between YANG-based service APIs and the OSS/BSS layer

The WG may decide that some documents such as problem statement. use-case, scope and priorities will remain as "living documents" rather than get published as RFCs.

## Relationship With Existing WGs

* Technology or protocol-specific modeling efforts (e.g., device-level YANG data models) remain the responsibility of their respective WGs.
* ONSEN WG will engage with other relevant WGs (e.g., NETMOD and NMOP) to gather requirements and input related to tooling.
* Any new requirements for changes to the YANG language that are identified during ONSEN WG discussions will be directed to the NETMOD WG for consideration.
* BESS/CCAMP/TEAS: ONSEN WG will take on future network and service data modeling efforts, while technology or protocol-specific modeling efforts remain in these WGs.
* NMOP: ONSEN WG will focus on abstractions, while topology-related efforts will remain in NMOP. Network topology models are out of scope of ONSEN.
* OPSAWG: ONSEN WG will handle AC/SAP/L2NM/L3NM work, enabling OPSAWG to focus on other operational topics. Future abstraction-related work will be directed to ONSEN.

## Milestones

| Date                      | Milestone | Description | Intended Track |
|---------------------------|-----------| -------------|:--------------:|
| June 2026              | Send LSes to TMF, 3GPP, BBF, GSMA, Linux Foundation, TIP, and EANTC about ONSEN | Actively seek collaboration with other organizations|N/A|
| November 2026              | WG adoption of a problem statement draft defining the use-cases, scope and priorities for the work items identified in the WG, with input operators, and the [IAB NEMOPS Workshop Report](https://datatracker.ietf.org/doc/draft-iab-nemops-workshop-report/). | Draft providing a problem statement draft to define use-cases, scope and priorities for the current set of ONSEN activities | Not published as RFC |
| December 2027                | WG adoption of a draft for Service-layer APIs based on YANG service models to interface with OSS/BSS | Draft detailing the Service-layer APIs based on YANG service models to interface with OSS/BSS | PS|
| December 2027                | WG adoption of a draft for new service and network level YANG data models as needed | Draft detailing service and network level YANG data models | PS |
| March 2027                | WG adoption of draft updating the YANG network data models for L3NM and L2NM | Updated drafts for L2NM and L3NM YANG data models based on operational feedback and deployment experiences, with attention to operational state data and identified gaps.| PS|
| March 2027                |WG adoption of draft that updates the YANG service data models for L3SM and L2SM |Updated drafts for L3SM and L3SM YANG data models based on operational feedback and deployment experiences, with attention to operational state data and identified gaps.| PS|
| July 2027                 |Submit document for Service-layer APIs based on YANG service models to interface with OSS/BSS to the IESG for publication as RFC. | Document detailing the Service-layer APIs based on YANG service models to interface with OSS/BSS | PS |