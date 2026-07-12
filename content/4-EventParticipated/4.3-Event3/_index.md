---
title: "Event 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# EVENT REPORT: FCAJ COMMUNITY DAY - "DATA DRIVEN, AI RISEN"

### Event Objectives
*   Delve into optimization methods for modern AI architectures, especially the application of Multi-agent systems in mitigating model hallucination.
*   Solve complex technical problems in Voice AI, particularly handling latency and the specific characteristics of the Vietnamese language.
*   Explore safe automated operations solutions (DevOps Agent) with a "Human-in-the-loop" mindset.
*   Understand how to deploy enterprise-grade AI systems (Amazon Q) accompanied by a closed security architecture via the MCP (Model Context Protocol).

### List of Speakers
*   **Steve Trần** - CTO/Founder, CloudThinker
*   **Trung Vũ** - CEO, Revve AI
*   **Trường Trần** - AI Solution Sales, Noventiq
*   **Anh Đặng** - Solution Sales, Noventiq
*   **Nghị Danh** - AI Engineer, Renova Cloud
*   **Kiệt Trần** - AI Engineer, AWS Student Builder Group
*   **Bảo Phan** - Cloud Engineer, Cloud Kinetics
*   **Nguyên Nguyễn** - Cloud Engineer, Cloud Kinetics
*   **Toàn Nguyễn** - AWS Security Builder

---

### Key Highlights

#### 1. AI Architecture Optimization (Steve Tran)
*   **Multi-agent architecture:** Separating agents by role (role-based agents) helps the model focus on specific data segments, thereby minimizing hallucination.
*   **"Champion Customer" strategy:** Instead of just doing proof-of-concept (PoC) projects, collaborating with large corporations (F88, FPT) provides valuable ground truth datasets to fine-tune the model.

#### 2. Voice AI & Natural Language Processing Techniques (Nghi Danh & Kiet Tran)
*   **Latency handling:** Applying partial streaming mechanisms to respond almost instantly, without waiting for the full response from the LLM.
*   **Vietnamese specifics & Barge-in:** Solving the prosody problem by training on 10-20% regional data. Notably, the system smoothly handles interruptions (barge-in), distinguishing between a user taking a breath and wanting to interrupt.

#### 3. DevOps Agent - Automated Operations (Bao Phan & Nguyen Nguyen)
*   **Root Cause Analysis (RCA) mechanism:** The AI automatically queries the Observability stack (Dynatrace), analyzes the topology, and compares it with incident history to generate hypotheses and validate them using logs.
*   **Absolute safety:** Although the AI can propose solutions, the system always requires human approval (human-in-the-loop) before executing changes on the production infrastructure.

#### 4. AI in HR & Data Management (Truong Tran & Anh Dang)
*   **Eliminating bias:** Amazon Q is provided with specialized skills to score resumes based on quantitative criteria (rubrics), integrating directly into the internal HRIS to automate the recruitment process.

#### 5. Security Architecture with MCP (Toan Nguyen & Nghi Danh)
*   **Private Networking:** Connecting the LLM to internal data sources via MCP in a Private Link environment. Data never leaves the VPC, ensuring absolute security compliance for the enterprise.
*   **The cost factor:** Deploying private infrastructure (Route 53 Resolver, ALB, EC2) entails additional operational costs (around $180 - $200+/month), requiring careful consideration between security and budget.

---

### What I Learned

#### Design Thinking
*   **Ground Truth mindset:** A powerful system does not lie in complex algorithms, but in the quality of the actual data used for training.
*   **Human-centric design (Human-in-the-loop):** Automation does not mean loosening control; every automated system that changes infrastructure configurations needs a human checkpoint.

#### Technical Architecture
*   **Optimizing closed network architecture:** Understanding the importance of Private Link and VPC in protecting the data communication flow between services and the AI Agent.
*   **Applying Observability:** Grasping how to exploit logs and metrics to automate the Root Cause Analysis (RCA) process in distributed systems.

---

### Application to Work & Project
*   **Protecting internal data:** Applying the Private Networking mindset to establish strict network boundaries within the VPC. Completely isolating the MySQL database and restricting the communication flow of Java Spring Boot APIs will thoroughly prevent unauthorized access.
*   **Optimizing system monitoring capabilities:** Applying RCA principles to establish a more systematic log structure for the N-Tier architecture. This accelerates the speed of tracking backend errors, ensuring stability for the application platform.
*   **Developing professional standards:** Applying the "human-in-the-loop" mindset when designing critical processing flows (such as booking and payment operations). This architectural and operational knowledge provides a solid foundation to meet the rigorous standards of the upcoming graduation internship and the real-world enterprise environment.

---

### Event Experience
Participating in the FCAJ Community Day at Bitexco Financial Tower was an excellent opportunity to approach "tough" technical problems in practical operations:
*   Expanding my perspective on how large corporations (like F88, FPT) process and integrate Generative AI into internal systems without compromising security standards.
*   Learning directly from engineers and solution experts from Noventiq, Renova Cloud, and Cloud Kinetics about the trade-offs between performance, cost, and safety when designing cloud architectures.

### Key Takeaways
*   In modern system architectures, applying AI (such as Multi-agent) not only speeds up processing but must also be designed with clear authorization to minimize the risk of data deviation.
*   Enterprise-grade security always comes with a cost factor. Technology selection (like MCP via Private Link) needs to be carefully calculated based on the core value and budget limits of the project.

---
### Event Photos

![Hình ảnh tham gia sự kiện 1](/fcaj-workshop/images/4-Event/event-27-6.avif) 

![Hình ảnh tham gia sự kiện 2](/fcaj-workshop/images/4-Event/event-27-6_minhchung.avif)