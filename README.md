# A2A-T
## Background
The interest group discusses the extension of interconnection protocols between agents applied in the telecommunications field, defined based on the A2A open-source project.
TM Forum Autonomous Network has released the IG1251C AN (Autonomous Network) functional architecture. This architecture defines three layers (business layer, service layer, network layer) and four closed loops (user closed-loop, business closed-loop, service closed-loop, network closed-loop), with each layer achieving automated closed-loop capabilities through agents.
The closed-loop of network management tasks in AN relies on agents, and interactions among multiple agents are unavoidable, including

- Cross layer interaction, i.e. Business layer, Service layer, Network layer’s interaction

- Cross domain interaction, i.e. cross domain fault management such as batch disconnection of wireless site

- Cross service interaction, i.e. cross domain fault management such as  IP optimization service triggers IP network expansion.

- Worker agents and supervisors or supervisory agents interaction, i.e. The task execution process involves dynamic permission requests or the review of potentially risky solutions.

## Issues and Scopes
Currently, two challenges exist regarding interconnection between agents.

- How Agents Connect？
  - The A2A open protocol provides a solution.
  - SDO like IETF are also working on developing standard protocols.
    
- How Agents Understand Each Other？
  - Different vertical industry contain distinct knowledge, and defining corresponding metamodel can effectively address this issue.
    
This project focuses on the mutual understanding of agents in autonomous network operations management tasks. After establishing interconnection between agents using the A2A open-source protocol, it aims to improve the interaction efficiency and accuracy of telecommunications operations management tasks by providing prompt templates for high-value AN scenarios.

## What are the challenges in understanding between agents?
The paper "Why Do Multi-Agent LLM Systems Fail", outlines the problems in understanding between agents.

| Category | Description | Example |
|---------|---------|---------|
| Specification and System Design Issues| These occur before the task is executed and are due to defects in the system design. | Ambiguous task descriptions, overlapping or conflicting role definitions of agents, and lack of clear termination conditions |
| Communication | These issues occur during task execution and stem from failures in communication and collaboration. | Agents withhold critical information, fail to clarify ambiguous instructions, or misinterpret the intentions of their peers |
| Verification | This occurs after task execution due to improper evaluation and closure. | The final results were not checked |

The O&M tasks make stricter requirements on the mutual understanding of agents

| Category | Description & Requirements |
|---------|---------|
| Specification and System Design Issues| - O&M tasks are highly Profession & Complexity <br> &nbsp;&nbsp; - Structured Prompt to balance accurate interaction of the structured interface and the ambiguity task processing capability of the natural language.<br>- The task boundaries between agents must be clearly defined.</br>|
| Communication | - O&M tasks require high real-time performance. <br> &nbsp;&nbsp; - Efficient negotiation mechanisms are needed for interpreting intents, assessing task feasibility, and handling resource conflicts. <br> &nbsp;&nbsp; - LLMs are based on prior knowledge, while the network is changing in real time. Mechanisms are needed to report network events in real time to correct deviations during task execution.|
| Verification | - High-risk operations must be reported for approval prior to execution to ensure operational correctness and goal alignment. |

## How to address?
The paper "Why Do Multi-Agent LLM Systems Fail", introduces the Methodology.

- Enhanced Communication Protocols: Develop standardized communication protocols that transform ambiguous natural language prompts into structured, verifiable formats to reduce semantic drift
- Quantification Mechanisms: Enable agents to assess and express their own uncertainty regarding tasks or information, and proactively request clarification when confidence falls below a threshold.
- Continuous Monitoring and Analysis: Treat agent interactions as observable data streams, enabling real-time analysis and feedback for early error correction.
- Verification Mechanisms: Implement layered verification that checks not only final outputs but also the correctness of intermediate steps and alignment with goals.

In TM Forum, a group of CSP and vendors propose the A2A-T IG1453 [File download link](https://www.tmforum.org/resources/introductory-guide/ig1453-agent-to-agent-protocol-for-telecoms-a2a-t-v2-0-0/) to provide a set of mechainsim based on above methodology, including, 

- Enhanced Communication Protocol: Provides structured prompts based on network tasks, transforming ambiguous natural language into structured, verifiable formats with a network ontology.
- Quantification Mechanism: Provides a set of negotiation mechanisms for task intent, task feasibility, resource conflicts, and dynamic information correction.
- Continuous Monitoring and Analysis: Real-time monitoring and feedback of network events to enable early deviation correction.
- Verification Mechanism: High-risk operations Review Mechanism

## Relationship to the A2A open-source project
This project does not aim to create a fork of A2A. It is intended solely for A2A-T participants to discuss and verify the soundness of the A2A-T standard, and to propose directions and potential solutions for its evolution. The outcomes of this project will be contributed back to the A2A project in compliance with the A2A extension governance.

## Participators
Michael Wang: wangzitao@huawei.com



