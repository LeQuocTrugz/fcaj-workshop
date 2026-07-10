---
title: "Worklog Week 11"
date: 2026-07-08
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Objectives for Week 11:

* Deploy the entire Football Field Booking project from the development environment (Local) to the actual production environment on the AWS ecosystem.
* Set up a Custom Domain to provide the application with a professional access address.
* Perform End-to-End Testing, evaluate stability, and finalize the final version of the project.

### Tasks to be implemented this week:

| Day | Task | Start Date | End Date | Resources |
| --- | --- | --- | --- | --- |
| Mon | - **Build actual AWS infrastructure:** <br>&emsp; + Create an EC2 virtual server located in the Public Subnet. <br>&emsp; + Initialize RDS MySQL in the Private Subnet to protect data. <br>&emsp; + Ensure the S3 Bucket is ready to store images. | 29/06/2026 | 29/06/2026 | |
| Tue | - **Configure EC2 environment:** <br>&emsp; + Use SSH to connect to the Linux server, install Java (Amazon Corretto/JDK). <br>&emsp; + Declare environment variables (FB_KEY, GG_KEY, DB_URL, DB_PASS) in the operating system's configuration file. | 30/06/2026 | 30/06/2026 | |
| Wed | - **Deploy source code to AWS:** <br>&emsp; + Transfer the packaged `.jar` file of the entire web project to the EC2 server. <br>&emsp; + Configure the web application to run stably as a background process. | 01/07/2026 | 01/07/2026 | |
| Thu | - **Configure Network & Domain:** <br>&emsp; + Finalize Firewall (Security Group) configurations for EC2 and RDS. <br>&emsp; + Register a custom domain and set up DNS records pointing successfully to the Public IP address of the EC2 instance. | 02/07/2026 | 02/07/2026 | |
| Fri | - **Testing & Finalize project:** <br>&emsp; + Access the system via the official domain, perform UAT testing for the entire business flow (Login, Field Booking, Image Upload). <br>&emsp; + Monitor system logs and finalize the project. | 03/07/2026 | 03/07/2026 | |


### Achievements in Week 11:

* **Successful deployment on a real environment:** Completed deploying the Spring Boot MVC project onto the AWS cloud platform. The application operates stably and smoothly 24/7 on the Linux server without interruption.
* **Professional Domain Integration:** Instead of accessing via a hard-to-remember IP address range, the system has been attached to an official Custom Domain, providing a professional user experience and a complete look similar to an actual commercial product.
* **Ensure Security & Connection:** System components communicate safely (EC2 connects securely to the private RDS and S3). All security keys (Client Keys) are strictly managed at the operating system level and are not leaked in the source code.
* **Project Completion:** Passed the final testing steps on the Production environment, officially finalizing the project and concluding the Workforce Bootcamp right on schedule.