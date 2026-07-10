---
title: "Worklog Week 5"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Objectives for Week 5:

* Deepen understanding of how EC2 virtual servers operate and how the system automatically scales (adds or removes servers) when user traffic fluctuates.
* Know how to configure automatic data backup features to mitigate risks and learn how to connect to cloud storage.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | Resources |
| --- | --- | --- | --- | --- |
| Mon | - **Theory study:** Watch the lecture video (Module 03) on the EC2 server service <br>&emsp; + Understand how to select appropriate instance types (CPU, RAM) for cost optimization | 11/08/2025 | 11/08/2025 |[Theory video](https://www.youtube.com/watch?v=e7XeKdOVq40&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=73)|
| Tue | - **Theory study:** Explore advanced features <br>&emsp; + Auto Scaling mechanism (prevents web crashes during high traffic) <br>&emsp; + Network file systems: EFS/FSx | 12/08/2025 | 12/08/2025 | [Theory video](https://www.youtube.com/watch?v=bbLcPitXJSY&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=79)|
| Wed |- **Practice:** Get familiar with AWS Backup <br>&emsp; + Manually configure an automated data backup schedule for the system instead of copying files manually | 13/08/2025 | 13/08/2025 | <https://000013.awsstudygroup.com/> |
| Thu |- **Practice:** <br>&emsp; + Perform a Test Restore to check if the backup is functioning properly, then delete it to avoid unnecessary charges | 14/08/2025 | 15/08/2025 | <https://000013.awsstudygroup.com/> |
| Fri | - **Practice:** Configure Storage Gateway <br>&emsp; + Use an EC2 instance as a "transit hub" to smoothly sync files directly to the S3 cloud storage | 15/08/2025 | 15/08/2025 | <https://000024.awsstudygroup.com/> |


### Achievements in Week 5:

* **Server Management:** Understood the operations and learned how to configure AWS virtual servers to automatically scale out when the system is overloaded.
* **Data Protection:** Not only knew how to automate backups but also successfully performed a manual test restore to ensure the system is always safe in the event of an incident.
* **Practical Storage:** Grasped how to seamlessly sync files from an on-premises (local) server directly to cloud storage (S3) via Storage Gateway.