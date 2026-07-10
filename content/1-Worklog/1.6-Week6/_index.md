---
title: "Worklog Week 6"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Objectives for Week 6:
* Know how to store data in the cloud with Amazon S3, from hosting a basic static website to advanced features like preventing accidental deletion and cross-region data replication.
* Know how to attach a Content Delivery Network (CloudFront) to make the website load fast everywhere and learn about solutions for migrating massive amounts of data to the cloud.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                        | Start Date | End Date   | Resources                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ----------------------------------------- |
| Mon | - **Theory study:** Watch Module 04 video about the AWS storage ecosystem <br>&emsp; + How to manage S3 access permissions (who can view, who is blocked) <br>&emsp; + Understand CORS rules                                 | 11/08/2025 | 11/08/2025 | [Theory video](https://www.youtube.com/watch?v=_yunukwcAwc&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=104) |
| Tue | - **Practice:** Run a website without a server <br>&emsp; + Create an S3 Bucket, upload static web source code (HTML/CSS/JS) <br>&emsp; + Configure public access so anyone can view the website                 | 12/08/2025 | 12/08/2025 | <https://000057.awsstudygroup.com/>       |
| Wed | - **Practice:** Accelerate the website with CDN <br>&emsp; + Integrate Amazon CloudFront into the newly created S3 website <br>&emsp; + Block direct access to S3, forcing users to go through CloudFront                     | 13/08/2025 | 13/08/2025 | <https://000057.awsstudygroup.com/>       |
| Thu | - **Practice:** Advanced S3 features <br>&emsp; + Enable Versioning (save old versions) to recover from accidental deletion <br>&emsp; + Configure Cross-Region Replication (CRR) to automatically replicate data to another Region      | 14/08/2025 | 15/08/2025 | <https://000057.awsstudygroup.com//>      |
| Fri | - **Theory study:** Data transfer methods <br>&emsp; + Broaden knowledge with the Snow family devices (Snowcone, Snowball, Snowmobile) <br>&emsp; + Review Storage Gateway and AWS Backup | 15/08/2025 | 15/08/2025 | [Theory video](https://www.youtube.com/watch?v=YXn8Q_Hpsu4&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=106) |


### Achievements in Week 6:
* **Static Web Hosting (Amazon S3):** Manually deployed a static website on the Internet running smoothly using only S3 without the cost of renting an entire server.
* **Acceleration & Security (CloudFront):** Knew how to hide the S3 bucket behind the scenes, integrating CloudFront as a Content Delivery Network (CDN) to help the web load faster via caching and prevent direct DDoS attacks.
* **Secure File Protection (Advanced S3):** Unlocked the "godsend" Versioning feature to recover accidentally overwritten or deleted files. Also knew how to configure Cross-Region Replication to automatically back up data to the other side of the globe.
* **Data Migration:** Grasped solutions to lift and shift a massive data center to the cloud using specialized physical devices (Snow Family) instead of spending time uploading over standard internet connections.