# Charter for Working Group — Network Management Operations (NMOP)

Source: https://datatracker.ietf.org/doc/charter-ietf-nmop/ (charter-ietf-nmop-01)

## Charter for Working Group

The increased drive by operators for integration and deployment of network management protocols and YANG data models may expose issues and problems with the individual protocols and models, or with the wider integration of both the protocols and the models. Some of these problems may only be witnessed when trying to manage large-scale networks, e.g., due to the increased complexity and handling large volumes of data exported in frequent updates.  At the same time, simplifying the network management and operations, with increased automation, is a high priority for network operators.

The goals of the Network Management Operations working group are to solicit input from network operators to identify existing and anticipated operational issues arising from the near-term deployment of network management technologies, and to consider potential solutions or workarounds for those issues.  Those operational issues may relate to deployments of existing network management technologies or the integration of related technologies for network management and telemetry.

Solving those operational issues requires discussion, investigation, and potentially some experiments, which may take some time.  However, the working group will focus on pragmatic items achievable in a short timeframe over long term architectural visions.

Since the focus is on solving network management problems faced by operators, discussion and experiments are not solely limited to network management technologies standardized within the IETF but may cover the wider network management ecosystem as it relates to the management of IETF protocols, subject to the following two constraints:

- The working group may discuss network management protocols and data models not standardized within the IETF only when they are being used to manage IETF protocols or to compare them to equivalent IETF solutions.

- The working group will not work on specific issues or improvements to protocols or data models developed and maintained outside the IETF. They must be taken to the appropriate organization for discussion and resolution.

The Network Management Operations working group is scoped, in rough order from highest to lowest priority, to:

- Present and discuss operational issues faced by the deployment of existing network management technologies.

- Discuss ideas for future short-term experiments (i.e., those focused on incremental improvements to network management operations that can be achieved in 1-2 years) and report on the progress of the relevant experimentation being done in the community.

- Discuss network operator use cases and requirements for solving anticipated problems related to the deployment of network management technologies.

- Standardize YANG data models to solve operational issues identified in the scope items above.  YANG data models potentially within the scope of other WGs will only be progressed here with agreement from the relevant ADs.

- Seek involvement with developers of open-source software to help drive adoption of IETF network management standards and to improve protocol maturity.

- Document operational experience and best practice for network management and telemetry deployment as BCPs or Informational RFCs.

This working group is not chartered to work on new protocols or protocol enhancements.

Agenda time at NMOP sessions at IETF meetings should allow for presentations and discussions of operator issues and experience, and other work within scope for the working group, but with a default expectation that priority be given to operator presentations.

The current topics of focus for the working group are:

- NETCONF/YANG Push integration with Apache Kafka & time series databases

- Anomaly detection and incident management

- Issues related to deployment/usage of YANG topology modules (e.g., to model a Digital Map)

- Consider/plan an approach for updating [RFC 3535](https://datatracker.ietf.org/doc/rfc3535/)-bis (collecting updated operator requirements for IETF network management solutions)

Like many of the "ops" working groups, this working group is expected to be long-lived, and is expected to remain open whilst there is sufficient interest and drive from the operators to work on topics within the scope described above.

---
_This file contains a Markdown copy of the NMOP WG charter from the IETF Datatracker. For the authoritative and up-to-date charter, see the Datatracker page above._
