---
title: "Worklog Week 7"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Objectives for Week 7:

* Understand the boundary of "who is responsible for what" when migrating a system to the cloud (Shared Responsibility Model).
* Grasp account management and user authorization tools (IAM, Cognito), and how to secure data using encryption.

### Tasks to be implemented this week:

| Day | Task | Start Date | End Date | Resources |
| --- | --- | --- | --- | --- |
| Mon | - **Theory study (Module 05):** <br>&emsp; + Explore the "Shared Responsibility Model" (simply put, AWS protects the physical infrastructure, while we are responsible for protecting our data and code). | 01/06/2026 | 01/06/2026 | [Theory video](https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150) |
| Tue | - **Theory study:** Access management services <br>&emsp; + Differentiate between IAM, AWS Organizations, and Identity Center. <br>&emsp; + Explore Amazon Cognito (a login mechanism similar to "Login with Google"). | 02/06/2026 | 02/06/2026 | [Theory video](https://www.youtube.com/watch?v=N_vlJGAqZxo&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=151) |
| Wed | - **Explore KMS & Practice (Lab):** <br>&emsp; + Enable the Security Hub service for security monitoring. <br>&emsp; + Check Security Standards and evaluate the Security Score by Standards. <br>&emsp; + Clean up resources. | 03/06/2026 | 03/06/2026 | <https://000018.awsstudygroup.com/> |
| Thu | - **Practice (Lab):** <br>&emsp; + Infrastructure preparation: Create VPC, Security Group, EC2 instance, and install Incoming Web-hooks for Slack. <br>&emsp; + Create Tags, assign Role to Lambda, write Lambda Function, and Check Result. <br>&emsp; + Clean up resources. | 04/06/2026 | 04/06/2026 | <https://000022.awsstudygroup.com/> |
| Fri | - **Practice (Lab):** <br>&emsp; + Use tags on Console: Create EC2 Instance with tag, manage and Filter resources by tag. <br>&emsp; + Experiment Using tags with CLI and Create a Resource Group. <br>&emsp; + Clean up resources. | 05/06/2026 | 05/06/2026 | <https://000027.awsstudygroup.com/> |


### Achievements in Week 7:

* **Cloud Security Mindset:** Understood the rules of the "Shared Responsibility Model," eliminating the dependency mindset that moving to the cloud means the system is automatically 100% secure.
* **Security Monitoring:** Manually enabled Security Hub for the first time to scan for vulnerabilities. Learned how to view Security Standards reports and assess risks via the Security Score by Standards. Did not forget the Clean Up Resources step to avoid incurring charges.
* **Automation & Alerts:** Completed a highly practical flow of a Cloud Engineer: Manually built VPC and EC2, then configured Incoming Web-hooks for Slack. Understood how to create a Role to grant permissions for a Lambda Function to run in the background and successfully push notifications to the chat channel (Check Result). Finally, performed Clean up resources.
* **Resource Management:** Realized the importance of Tagging when the system has too many servers. Mastered creating an EC2 Instance with tag, and Filter resources by tag on both the Console interface and CLI. Grasped how to cluster resources using Create a Resource Group and neatly executed Clean up resources.