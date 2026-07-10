---
title: "Worklog Week 9"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Objectives for Week 9:

* Brainstorm, discuss with the team, and finalize the topic for the capstone internship project.
* Analyze requirements, sketch the system architecture diagram on **draw.io**, conduct a review, discuss with the Mentor, and refine it to achieve the most optimal design.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                        | Start Date | End Date   | Resources                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ----------------------------------------- |
| Mon | - **Idea Generation:** <br>&emsp; + Brainstorm feasible topics. <br>&emsp; + Discuss with the team and officially finalize the topic: **Building a Football Field Booking Management System**. | 15/06/2026 | 15/06/2026 |                                           |
| Tue | - **Requirement Analysis:** <br>&emsp; + List core features (Search fields, booking, payment, user management). <br>&emsp; + Preliminary design of the Database Schema for the system.                 | 16/06/2026 | 16/06/2026 |                                           |
| Wed | - **AWS Architecture Design (Draft 1):** <br>&emsp; + Apply learned knowledge to draw the system flow. <br>&emsp; + Discuss with the team to identify errors that need fixing.                 | 17/06/2026 | 17/06/2026 | Draw.io                                   |
| Thu | - **Design Review & Troubleshooting:** <br>&emsp; + Present the draft diagram to the Mentor and team. <br>&emsp; + **Error Detected:** Incorrect Database security flow and missing secure internal connection Endpoints.                     | 18/06/2026 | 18/06/2026 |                                           |
| Fri | - **Finalize Overall Architecture:** <br>&emsp; + Revise the diagram: Add S3 Gateway Endpoint and RDS Endpoint. <br>&emsp; + Update the Multi-AZ mechanism for the Database. <br>&emsp; + Finalize the ultimate AWS architecture drawing.      | 19/06/2026 | 19/06/2026 | Draw.io                                   |

### Achievements in Week 9:
* **Topic Finalization:** Clearly defined the objectives and scope of the "Football Field Booking System" project, creating a solid stepping stone for the coding phase.
* **System Design Thinking:** Through the process of "drawing - making mistakes - redrawing", I gained a deeper understanding of why a Gateway Endpoint must be used instead of routing through the Internet, and the importance of placing the Database in a closed Private Subnet. The final AWS architecture diagram was approved by the Mentor and is ready for actual deployment.