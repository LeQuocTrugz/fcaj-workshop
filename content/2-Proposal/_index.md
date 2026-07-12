---
title: "Proposal"
date: 2026-07-04
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

In this section, you need to summarize the contents of the workshop you intend to execute.

# Sports Field Booking System Project
## AWS High Availability & Scalable Architecture Deployment Solution

### 1. Executive Summary
The Sports Field Booking System is designed to provide a stable, secure, and highly available web platform for users. The platform utilizes AWS architecture with complete separation of the Frontend (static) and Backend (dynamic), leveraging Auto Scaling capabilities across multiple Availability Zones (Multi-AZ). This solution ensures the system operates smoothly even during peak hours, optimizes operational costs, and ensures data security with Amazon RDS and in-depth security layers like AWS WAF.

### 2. Problem Statement
**Current Issues**
Traditional sports field booking systems often experience overload, slow responses, or crashes during golden hours (e.g., 17:00 - 19:00). Centralized storage on a single server (Single Point of Failure) poses a risk of data loss, while the cost of maintaining high-configuration servers 24/7 wastes budget when the system has low traffic.

**Solution**
The project applies a Cloud-native architecture on AWS. The frontend is statically hosted on Amazon S3 and delivered at high speed via CloudFront. The backend logic is directly processed by a cluster of EC2 instances (using Java Spring Boot) located in a Private Subnet, managed by an Application Load Balancer (ALB) and an Auto Scaling Group. The MySQL database is hosted on Amazon RDS using a Multi-AZ model (with a Standby replica) to prevent failures. The system is also continuously monitored by CloudWatch with alerts sent via SNS.

**Benefits and Return on Investment (ROI)**
This architecture provides up to 99.9% Uptime, enhancing the end-user booking experience. The system only scales out computing resources during high traffic and scales in when idle, maximizing infrastructure cost savings. Additionally, maintenance and upgrades happen seamlessly due to the distributed architecture, causing no service interruptions.

### 3. Solution Architecture
The platform applies an AWS architecture combining Serverless (for Frontend/Storage) and Auto-scaling Instances (for Backend/Database) across 2 Availability Zones (AZ A and AZ B).

**Data Flow:**

![Sports Field Booking System Project](/fcaj-workshop/images/2-Proposal/anh_kien_truc.png)

- **Access & Security (1)**: Users access the domain resolved by Route 53. Traffic passes through CloudFront (CDN) and is securely inspected by AWS WAF.
- **Frontend (3)**: CloudFront retrieves static UI data (ReactJS/Vue/HTML...) from the FE Static S3 bucket.
- **Backend Routing (2, 4)**: API requests pass through the Internet Gateway (IGW) to the Internet-facing ALB. The ALB distributes the load to the Target Group.
- **Logic Processing (5)**: The Target Group routes requests to EC2 instances located in the Auto Scaling Group within the Private Subnet of AZ A or AZ B. These servers use a NAT Gateway in the Public Subnet to access the Internet when necessary (e.g., calling third-party payment APIs).
- **Database (6)**: EC2 connects to Amazon RDS MySQL (Primary). Data is continuously synchronized to the Standby replica in AZ B (Multi-AZ) to ensure safety.
- **Backend Static Storage (7)**: Files uploaded by users (field images, invoices, avatars) are pushed by EC2 to the BE S3 bucket.
- **Monitoring & Alerting (8)**: The status of RDS and the system is collected by CloudWatch; if an issue occurs, it triggers AWS SNS to send alert emails to administrators.

**Main AWS Services Used**
- **Amazon Route 53, CloudFront & WAF**: Manage DNS, accelerate page load times, and protect the system from common web attacks (e.g., DDoS, SQL Injection).
- **Application Load Balancer (ALB) & Auto Scaling Group**: Load balancing and automatically scaling the number of EC2 instances up or down.
- **Amazon EC2**: Run the Backend application (Java Spring Boot, Hibernate).
- **Amazon RDS (MySQL, Multi-AZ)**: Relational database management with automatic failover during incidents.
- **Amazon VPC, NAT Gateway, IGW**: Build a virtual private network, separating Public and Private environments for absolute security of the Backend and DB.
- **Amazon S3**: Store the static Frontend (FE Static S3) and system files (BE S3).
- **Amazon CloudWatch & SNS**: Monitor resources, log data, and automatically send notifications via Email.

### 4. Technical Implementation
**Deployment Phases**
The project is divided into 4 main phases to deploy the application on AWS:

1. **Basic Network & Storage Setup**: Configure VPC, divide Subnets (Public/Private), set up IGW, NAT Gateway, and S3 buckets. Push static Frontend code to S3.
2. **Database & Server Configuration**: Initialize Amazon RDS MySQL (Multi-AZ). Configure Launch Templates for EC2 containing the Java/Node.js runtime environment, set up the Auto Scaling Group and ALB.
3. **Edge Network & Security Deployment**: Connect Route 53 with the domain name, configure CloudFront to distribute the Frontend S3, and attach AWS WAF to protect the ALB/CloudFront.
4. **Monitoring & Optimization**: Set up monitoring metrics on CloudWatch, configure SNS to send emails when EC2 is overloaded or RDS encounters errors. Configure CI/CD to automatically deploy new code.

**Technical Requirements**
- **Frontend**: Built as static files (HTML/CSS/JS) optimized for S3 static website hosting.
- **Backend**: The application (e.g., Java Spring Boot) must follow Stateless standards (no session stored on the server, using JWT) for Auto Scaling to work correctly. Run on port 80/8080 for ALB health checks.
- **Database**: Use MySQL with Hibernate/JPA connections, configure optimal connection pools to handle load from multiple EC2 instances simultaneously.

### 5. Roadmap & Deployment Milestones
- **Week 1: Finalize Local & Initialize Infrastructure**
  - Complete coding and testing of the Sports Field Booking system functionalities (static UI and Java Spring Boot backend) in the local environment.
  - Create an AWS account, design the core network (VPC, Public/Private Subnets, Internet Gateway).
- **Week 2: Data & Edge Network Deployment**
  - Initialize and configure the MySQL database on Amazon RDS.
  - Upload static Frontend source code to the S3 bucket and configure high-speed content delivery via CloudFront.
- **Week 3: Backend Deployment & Auto Scaling**
  - Package the Backend application, create a Launch Template, and set up the EC2 Auto Scaling cluster.
  - Configure the Application Load Balancer (ALB) to securely route traffic to the Backend.
- **Week 4: Completion, Testing & Reporting**
  - Integrate the actual domain name (Route 53) and set up system monitoring and alerts via CloudWatch combined with SNS.
  - Perform load testing, review cost optimization, and finalize the project report.

### 6. Budget Estimation
You can find the budget estimation on the [AWS Pricing Calculator](https://calculator.aws/#/estimate?id=621f38b12a1ef026842ba2ddfe46ff936ed4ab01).  
Or you can download the [Budget Estimation File](../attachments/budget_estimation.pdf).

**Infrastructure Costs (Estimated)**
- Application Load Balancer (ALB): ~16.50 USD/month.
- Amazon EC2 (2 t3.micro instances in Auto Scaling): ~15.00 USD/month.
- Amazon RDS (MySQL t3.micro, Multi-AZ): ~34.00 USD/month.
- NAT Gateway (1 instance): ~32.00 USD/month.
- Amazon S3 & CloudFront (Low traffic): ~2.00 USD/month.
- Route 53 (1 Hosted Zone): 0.50 USD/month.
- AWS WAF, CloudWatch, SNS: Within Free Tier or ~3.00 USD/month.

*Total: Approximately 103.00 USD/month.*

### 7. Risk Assessment
**Risk Matrix**
- **DDoS Attack or Web Exploit**: High impact, medium probability.
- **Database overload due to complex queries**: High impact, high probability (during sudden booking surges).
- **Exceeding AWS budget (Cloud Shock)**: High impact, medium probability.

**Mitigation Strategies**
- **Security**: Use AWS WAF to block malicious IPs, Rate Limiting on CloudFront/ALB. Place DB and Backend in a Private Subnet, do not assign public IPs.
- **Database**: Utilize Read Replicas (if read scaling is needed), optimize MySQL indexes, use Hibernate Caching.
- **Cost**: Set up AWS Budgets to immediately alert if costs exceed $10 or $20 thresholds. Turn off EC2 instances and RDS at night when not developing.

### 8. Expected Outcomes
- **Technical Improvements**: The system automatically scales to handle thousands of concurrent visits without crashing. Ultra-fast loading interface thanks to CloudFront CDN.
- **Project Value**: Demonstrates practical cloud deployment capabilities with enterprise standards (High Availability, Fault Tolerance, Secure by Design), creating a stepping stone for applying to Backend/DevOps positions.