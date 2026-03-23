## Key Feature for A2A in ICT Area

In the ICT field, tasks exhibit several common characteristics and requirements.

- **Profession & Complexity**: ICT tasks are highly specialized and complex. For example, in fault management, wireless faults alone can be categorized into 15 major types with 189 root causes. At the same time, not all faults generate alarms, which requires specialized diagnosis and repair capabilities. The interaction among functional modules must be accurate and efficient. Additionally, network services involve extensive cross-layer, cross-domain, and cross-service interactions, requiring robust solutions for handling complex and ambiguous tasks.

- **Real-time**: these tasks demand real-time processing. Phenomena such as network traffic tidal effects, holidays, major events, and hotspot incidents cause rapid changes in network status, necessitating real-time adaptive corrections to enhance response efficiency.

- **Security**: Networks deal with vast amounts of privacy and sensitive data. As agent capabilities grow, ensuring their security and trustworthiness becomes essential. Especially, the use of agentic AI solutions has introduced numerous new attack vectors, and efforts are still underway to find solutions that ensure security within the operational paradigm. This requires not only basic security authentication but also mechanisms to log agent-involved tasks and collaborative activities, enabling traceability and accountability.

---

## Gap Analysis

As outlined above, in the ICT domain, agent communication protocols must meet the following requirements:

- Ensuring the security and traceability of agent interactions
- Providing task-based multi-round negotiations to enable dynamic corrections and address real-time network issues
- Balancing the accuracy of structured language with the efficiency of natural language processing to handle ambiguous tasks

These criteria are essential to effectively address the professional and complex challenges inherent in ICT tasks.

This document analyzes the gap between the capabilities of the A2A protocol and the interaction requirements of agents in the ICT domain, as shown in the table below.

| Requirements | A2A |
|--------------|-----|
| Registration & Discovery | √ |
| Agent Description | √ |
| Task Status | √ |
| Task Processing | √ |
| Efficiency and professional prompt and self-explanatory terminologies in ICT area | • JSON format, supporting text, structured data, and multimodal data. |
| Task negotiation to provide dynamic correction capabilities | • Only support negotiation of user interface capabilities, such as iframes, videos, and web forms |
| Transmission Protocol, TMF support HTTP+RESTFUL | √ |
| Subscription & Notification | √ |
| Security governance and traceability | • supports various authentication methods including HTTP Basic Auth, API Key, and OAuth 2.0. |


