---
title: "Worklog Week 4"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Objectives for Week 4:

* Master the concepts of multi-layer network security on AWS (Security Groups, Network ACLs) and the VPC Resource Map network visualization tool.
* Practice building a complete custom cloud network (Custom VPC) from scratch, including routing configuration, traffic monitoring, and secure remote access setup.

### Tasks to be implemented this week:

| Day | Task | Start Date | End Date | Resources |
| --- | --- | --- | --- | --- |
| Mon | - **Theory study:** Deep dive into AWS network security <br>&emsp; + Differentiate between Security Groups (Stateful) and Network ACLs (Stateless) <br>&emsp; + Read and understand network diagrams via VPC Resource Map | 11/05/2026 | 11/05/2026 | [Theory video](https://www.youtube.com/watch?v=BPuD1l2hEQ4&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=26) |
| Tue | - **Practice (Lab):** Build basic network infrastructure <br>&emsp; + Initialize Custom VPC <br>&emsp; + Subnet division (Public and Private) <br>&emsp; + Attach Internet Gateway and configure Route Tables | 12/05/2026 | 12/05/2026 | <https://000003.awsstudygroup.com/> |
| Wed | - **Practice (Lab):** Set up security & Network monitoring <br>&emsp; + Create and attach Security Groups for resources <br>&emsp; + Enable VPC Flow Logs to trace network traffic | 13/05/2026 | 13/05/2026 | <https://000003.awsstudygroup.com/> |
| Thu | - **Practice (Lab):** Outbound network communication <br>&emsp; + Deploy EC2 into the newly created network <br>&emsp; + Configure NAT Gateway <br>&emsp; + Check connectivity using Reachability Analyzer | 14/05/2026 | 15/05/2026 | <https://000003.awsstudygroup.com/> |
| Fri | - **Practice (Lab):** Set up remote access <br>&emsp; + Configure EC2 Instance Connect Endpoint (EICE) <br>&emsp; + Test secure SSH connection to Private EC2 without a Public IP | 15/05/2026 | 15/05/2026 | <https://000003.awsstudygroup.com/> |


### Achievements in Week 4:

* **Network Security & Monitoring:** Understood the differences and how to combine Security Groups and Network ACLs. Successfully enabled VPC Flow Logs to monitor data flow and used VPC Resource Map to visualize the architecture.
* **Basic Network Infrastructure Deployment (VPC & Routing):** Manually drafted and successfully configured a complete network environment including Custom VPC, splitting Public/Private Subnets, Internet Gateway, and Route Tables.
* **Secure Outbound Communication (NAT Gateway):** Deployed a NAT Gateway allowing virtual servers (EC2) located in the Private Subnet to securely access the internet for software updates; applied Reachability Analyzer to test and debug network flows.
* **Secure Remote Access:** Successfully established an EC2 Instance Connect Endpoint, creating a secure tunnel that allows direct connection (SSH) to virtual servers in the internal network without having to open ports or assign a Public IP to the Internet.