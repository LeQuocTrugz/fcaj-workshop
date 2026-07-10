---
title: "Worklog Week 2"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Objectives for Week 2:

* Master the theory of core AWS services, including: Identity and Access Management (IAM), Amazon Elastic Compute Cloud (Amazon EC2), and Amazon Elastic Block Store (Amazon EBS).
* Apply theoretical knowledge into hands-on practice (Labs) to manually initialize and configure resources on AWS.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                        | Start Date | End Date   | Resources                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ----------------------------------------- |
| Mon | - **Theory study:** Research lecture videos on Identity and Access Management (IAM) <br>&emsp; + Concepts of Users, Groups, Roles, Policies <br>&emsp; + Security best practices                                  | 27/04/2026 | 27/04/2026 | <https://000002.awsstudygroup.com/>       |
| Tue | - **Practice:** <br>&emsp; + Practice creating an IAM User account <br>&emsp; + Assign permissions (attach Policy) and securely set up password and MFA for the IAM User                                          | 28/04/2026 | 28/04/2026 | <https://000002.awsstudygroup.com/2-create-admin-user-and-group/> |
| Wed | - **Theory study:** Research lecture videos on Virtual Servers (Amazon EC2) and Virtual Hard Drives (Amazon EBS) <br>&emsp; + Various Instance Types <br>&emsp; + EBS operating mechanism                     | 29/04/2026 | 29/04/2026 | <https://000004.awsstudygroup.com/>       |
| Thu | - **Practice:** <br>&emsp; + Initialize and configure an EC2 virtual server (select AMI, Instance Type, Key Pair) <br>&emsp; + Run the server and verify SSH/SSM connections                                      | 30/04/2026 | 30/04/2026 | <https://000003.awsstudygroup.com/4-createec2server/> |
| Fri | - **Practice:** <br>&emsp; + Create a new virtual hard drive (EBS volume) <br>&emsp; + Attach the drive to a running EC2 instance <br>&emsp; + Format the hard drive within the OS                                | 01/05/2026 | 01/05/2026 | <https://000003.awsstudygroup.com/4-createec2server/> |


### Achievements in Week 2:

* Mastered AWS security mechanisms and permission management through the IAM service.
* Successfully initialized and configured IAM Users, assigning permissions adhering to the "Least Privilege" principle.
* Clearly understood the concepts and operational lifecycle of a cloud virtual server (Amazon EC2).
* Manually initialized, configured the network and security (Security Groups), and successfully established a connection to the EC2 server.
* Grasped how to expand storage space for the server by successfully creating, attaching, and formatting a virtual hard drive (EBS volume) while the instance is actively running.