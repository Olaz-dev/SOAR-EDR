# SOAR-EDR

## Objective
The SOAR EDR lab project aimed at creating an automatic procedure to respond to incidents with Tines SOAR and LimaCharlie EDR by identifying potentially dangerous password recovery software on Windows devices, providing real-time alerts through Slack from the telemetry and allowing for automated triaging, host isolation, etc... Also validated detection criteria and playbook performance through mock credential dumping attacks; developed practical experience converting detection events into coordinated incident response.

### Skills Learned
- SOAR Workflow Automation with Tines
- EDR Detection Rule Development in LimaCharlie
- Credential Dumping Detection (LaZagne)
- Real-time Slack Alerting & User Prompts
- Automated Endpoint Isolation
- LimaCharlie Telemetry Integration
- Attack Simulation & Workflow Validation
- SOAR Story Design & Workflow Diagramming

### Tools Used

<img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white" />​
<img src="https://img.shields.io/badge/LimaCharlie-0A2540?style=for-the-badge&logo=lima-charlie&logoColor=white" />​
<img src="https://img.shields.io/badge/LaZagne-FF6B35?style=for-the-badge&logo=lazagne&logoColor=white" />​
<img src="https://img.shields.io/badge/Atomic_Red_Team-EE0000?style=for-the-badge&logo=atomic-red-team&logoColor=white" />
<img src="https://img.shields.io/badge/-Tines-0A2540?style=for-the-badge&logo=tines&logoColor=white" />
<img src="https://img.shields.io/badge/-Virtualization%20&%20Testing_Windows_VMs-0A2540?style=for-the-badge&logo=virtualbox&logoColor=white" />

## Steps and Images
Created detailed workflow diagrams to map SOAR playbooks and iteratively refine automation logic during design and deployment.
​

Deployed custom detection rule in LimaCharlie to identify credential dumping tools (LaZagne) and trigger automated playbook responses.
​

Integrated LimaCharlie telemetry with Tines via webhook for real-time SOAR story execution and automated triage.
​

Designed Tines SOAR "story" for Slack alerts, email notifications, user prompts, and conditional host isolation based on analyst feedback.
​

Configured Slack as interactive communication layer in SOAR workflow for decision-making and response execution.
​

Simulated real-world password recovery attack using LaZagne on monitored Windows VM to generate telemetry.
​

Validated end-to-end detection-response workflow, confirming alerts, isolation, and telemetry flow.



Work Flow (Draw.io)
<img width="1837"  height="719" alt="WorkFlow_diagram" src="https://github.com/user-attachments/assets/3804a866-649e-4643-a2f6-413cb5368e59" />

EDR Rule (Lima Charlie)
<img width="1532" height="755" alt="EDr Rule Created" src="https://github.com/user-attachments/assets/8430c30c-6f9d-4626-882b-9c5820c8af03" />

Host Isolated (Lima Charlie)
<img width="1915" height="986" alt="HostIsolated" src="https://github.com/user-attachments/assets/d70dfb18-e4c9-400f-8a79-9222c15e0b51" />

Lazagne Execution (Powershell)
<img width="1014" height="768" alt="LazagneExecution" src="https://github.com/user-attachments/assets/c3c42af0-68b9-402c-bcf8-dd151816668c" />

Isolation Pending (Lima Charlie)
<img width="1900" height="862" alt="IsolationPending" src="https://github.com/user-attachments/assets/6dcbbf21-a6d5-4592-9d34-91212fecd564" />

Slack Message (Host Isolated)
<img width="1915" height="860" alt="SlackShowingCompleteEdr" src="https://github.com/user-attachments/assets/2859c12a-b2ac-46eb-b9c1-600c31b8b3af" />

D&R Creation (Lima Charlie)
<img width="1900" height="862" alt="rulecreation" src="https://github.com/user-attachments/assets/f4724fb2-a3b4-4aa6-ab67-c61d4bf76b3e"/>
<img width="1919" height="988" alt="LimaCharlieSetup" src="https://github.com/user-attachments/assets/815c3ed1-32f6-4bb4-a3a8-fc2b1f95f986" />

Isolation Completed (Lima Charlie)
<img width="1900" height="862" alt="IsolationPending" src="https://github.com/user-attachments/assets/ade55a4e-54db-4fc9-adfb-a80d348ddf84" />

Automation Workflow (Tine)
<img width="1900" height="862" alt="tineworkflow" src="https://github.com/user-attachments/assets/8ed94942-4c1d-4be6-8bd2-298cf0322cbb" />

Workflow Setup (Tine)
<img width="1900" height="862" alt="tineworkflow" src="https://github.com/user-attachments/assets/3eeeb1f6-698e-4e90-90a5-2ab06fc2409f" />

