---
title: "Worklog Week 8"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Objectives for Week 8:

* Review database fundamentals and get acquainted with AWS cloud data storage services such as RDS, Aurora, Redshift, and ElastiCache.
* Practice deploying an application connected to a Database and learn how to migrate entire datasets from one location to another using AWS DMS.

### Tasks to be implemented this week:

| Day | Task | Start Date | End Date | Resources |
| --- | --- | --- | --- | --- |
| Mon | - **Theory study:** <br>&emsp; + Review core database concepts. <br>&emsp; + Explore Amazon RDS and Amazon Aurora architecture. | 08/06/2026 | 08/06/2026 | [Theory video](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) |
| Tue | - **Theory study:** <br>&emsp; + Research specialized data solutions: Amazon Redshift (massive data warehouse) and ElastiCache (caching mechanism to accelerate web data read speed). | 09/06/2026 | 09/06/2026 | [Theory video](https://www.youtube.com/watch?v=UvdiRW34aNI&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=219) |
| Wed | - **Practice (Lab):** <br>&emsp; + Infrastructure preparation: Create EC2 instance and Create RDS database instance. <br>&emsp; + Application Deployment (install app and connect to DB). <br>&emsp; + Test Backup and Restore. | 10/06/2026 | 10/06/2026 | <https://000005.awsstudygroup.com/> |
| Thu | - **Practice (Lab):** <br>&emsp; + Get familiar with the AWS DMS tool. <br>&emsp; + Configure input/output: Select your DMS source & Select your DMS Target. <br>&emsp; + Launch Serverless replication to copy data. | 11/06/2026 | 11/06/2026 | <https://000043.awsstudygroup.com/> |
| Fri | - **Practice (Lab):** <br>&emsp; + Monitoring DMS Migrations (track the data transfer process). <br>&emsp; + Troubleshooting Migrations (practice debugging and handling errors). <br>&emsp; + Clean up resources & Environment Cleanup. | 12/06/2026 | 12/06/2026 | <https://000043.awsstudygroup.com/> |


### Achievements in Week 8:

* **Relational Database Management System (RDS):** Understood clearly how AWS operates databases. With this knowledge, I successfully initialized a standard Amazon RDS MySQL cluster and configured strict Security Groups to prepare for connecting with Backend APIs later.
* **Speed Optimization & Analytics (ElastiCache & Redshift):** Broadened my mindset on how large systems handle millions of requests via caching mechanisms and how to store data for analytics and statistics (Data Warehouse).
* **Hands-on App Deployment (Lab 05):** Completed the practical loop of a Backend Developer: Set up a server (EC2), set up a Database (RDS), push the application code (Application Deployment), and connect them together. Additionally, manually tested the Backup and Restore feature to ensure data is not lost during incidents.
* **Data Migration (Lab 43):** Mastered the skill of database migration using AWS DMS. Learned how to set up the Source, Target, and specifically how to read logs (Monitoring & Troubleshooting) to find the root cause if the data transfer process is interrupted.