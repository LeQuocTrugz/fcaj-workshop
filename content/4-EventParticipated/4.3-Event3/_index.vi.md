---
title: "Event 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# BÀI THU HOẠCH: FCAJ COMMUNITY DAY - "DATA DRIVEN, AI RISEN"

### Mục Đích Của Sự Kiện
*   Đi sâu vào các phương pháp tối ưu hóa kiến trúc AI hiện đại, đặc biệt là ứng dụng Multi-agent trong việc giảm thiểu ảo tưởng (hallucination) của mô hình.
*   Giải quyết các bài toán kỹ thuật phức tạp trong Voice AI, đặc biệt là xử lý độ trễ (latency) và đặc thù ngôn ngữ tiếng Việt.
*   Khám phá các giải pháp tự động hóa vận hành an toàn (DevOps Agent) với tư duy "Human-in-the-loop".
*   Hiểu rõ cách triển khai các hệ thống AI cấp doanh nghiệp (Amazon Q) đi kèm với kiến trúc bảo mật khép kín thông qua giao thức MCP (Model Context Protocol).

### Danh Sách Diễn Giả
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

### Nội Dung Nổi Bật

#### 1. Tối ưu hóa kiến trúc AI (Steve Trần)
*   **Kiến trúc Multi-agent:** Tách biệt các tác tử theo vai trò (role-based agents) giúp mô hình tập trung vào từng phân khúc dữ liệu chuyên biệt, từ đó giảm thiểu tối đa hiện tượng hallucination.
*   **Chiến lược "Champion Customer":** Thay vì chỉ làm các dự án thử nghiệm (PoC), việc hợp tác với các tập đoàn lớn (F88, FPT) mang lại tập dữ liệu thực tế (ground truth) quý giá để tinh chỉnh (fine-tune) mô hình.

#### 2. Kỹ thuật Voice AI & Xử lý ngôn ngữ tự nhiên (Nghị Danh & Kiệt Trần)
*   **Xử lý độ trễ:** Ứng dụng cơ chế streaming từng phần để phản hồi gần như tức thì, không cần chờ toàn bộ câu trả lời từ LLM.
*   **Đặc thù tiếng Việt & Barge-in:** Giải quyết bài toán ngữ điệu (prosody) bằng cách huấn luyện 10-20% dữ liệu vùng miền. Đặc biệt, hệ thống xử lý mượt mà tình huống ngắt lời (barge-in), phân biệt được khi người dùng lấy hơi hay muốn cắt ngang.

#### 3. DevOps Agent - Tự động hóa vận hành (Bảo Phan & Nguyên Nguyễn)
*   **Cơ chế Root Cause Analysis (RCA):** AI tự động truy vấn Observability stack (Dynatrace), phân tích topology và so sánh với lịch sử sự cố để đưa ra giả thuyết và kiểm chứng bằng logs.
*   **An toàn tuyệt đối:** Dù AI có khả năng đề xuất giải pháp, hệ thống luôn yêu cầu bước phê duyệt của con người (human-in-the-loop) trước khi thực thi thay đổi trên hạ tầng sản xuất.

#### 4. AI trong HR & Quản trị dữ liệu (Trường Trần & Anh Đặng)
*   **Loại bỏ định kiến:** Amazon Q được cấp các skill chuyên biệt để chấm điểm hồ sơ dựa trên các tiêu chí (rubrics) định lượng, tích hợp trực tiếp vào hệ thống HRIS nội bộ nhằm tự động hóa quy trình tuyển dụng.

#### 5. Kiến trúc bảo mật với MCP (Toàn Nguyễn & Nghị Danh)
*   **Private Networking:** Kết nối LLM với nguồn dữ liệu nội bộ thông qua MCP trong môi trường Private Link. Dữ liệu không bao giờ rời khỏi VPC, đảm bảo tuân thủ bảo mật tuyệt đối cho doanh nghiệp.
*   **Bài toán chi phí:** Triển khai hạ tầng private (Route 53 Resolver, ALB, EC2) kéo theo chi phí vận hành tăng thêm (khoảng 180$ - 200$+/tháng), đòi hỏi sự cân nhắc kỹ lưỡng giữa bảo mật và ngân sách.

---

### Những Gì Học Được

#### Tư Duy Thiết Kế
*   **Tư duy dữ liệu thực tế (Ground Truth):** Một hệ thống mạnh mẽ không nằm ở thuật toán phức tạp, mà ở chất lượng dữ liệu thực tế được sử dụng để huấn luyện.
*   **Thiết kế lấy con người làm trung tâm (Human-in-the-loop):** Tự động hóa không đồng nghĩa với buông lỏng kiểm soát; mọi hệ thống tự động thay đổi cấu hình hạ tầng đều cần có điểm chốt chặn của con người.

#### Kiến Trúc Kỹ Thuật
*   **Tối ưu hóa kiến trúc mạng kín:** Hiểu rõ tầm quan trọng của Private Link và VPC trong việc bảo vệ luồng dữ liệu giao tiếp giữa các service và AI Agent.
*   **Ứng dụng Observability:** Nắm bắt cách khai thác logs và metrics để tự động hóa quá trình tìm kiếm nguyên nhân gốc rễ (RCA) trong các hệ thống phân tán.

---

### Ứng Dụng Vào Công Việc & Đồ Án
*   **Bảo vệ dữ liệu nội bộ:** Áp dụng tư duy Private Networking để thiết lập các giới hạn mạng chặt chẽ trong VPC. Việc cô lập hoàn toàn cơ sở dữ liệu MySQL và giới hạn luồng giao tiếp của các API Java Spring Boot sẽ ngăn chặn triệt để các truy cập trái phép.
*   **Tối ưu hóa khả năng giám sát hệ thống:** Vận dụng các nguyên lý phân tích RCA (Root Cause Analysis) để thiết lập cấu trúc log bài bản hơn cho kiến trúc N-Tier. Điều này giúp đẩy nhanh tốc độ truy vết lỗi backend, đảm bảo độ ổn định cho nền tảng ứng dụng.
*   **Phát triển chuẩn mực nghề nghiệp:** Áp dụng tư duy "human-in-the-loop" khi thiết kế các luồng xử lý quan trọng (như nghiệp vụ booking, thanh toán). Những kiến thức kiến trúc và vận hành này là hành trang vững chắc đáp ứng các tiêu chuẩn khắt khe cho kỳ thực tập tốt nghiệp và môi trường doanh nghiệp thực tế.

---

### Trải Nghiệm Trong Sự Kiện
Tham gia FCAJ Community Day tại Bitexco Financial Tower là một cơ hội tuyệt vời để tiếp cận những bài toán kỹ thuật "khó nhằn" trong thực tế vận hành:
*   Mở rộng tầm nhìn về cách các doanh nghiệp lớn (như F88, FPT) xử lý và tích hợp Generative AI vào hệ thống nội bộ mà không thỏa hiệp với các tiêu chuẩn bảo mật.
*   Học hỏi trực tiếp từ các kỹ sư và chuyên gia giải pháp đến từ Noventiq, Renova Cloud, Cloud Kinetics về những đánh đổi (trade-offs) giữa hiệu năng, chi phí và mức độ an toàn khi thiết kế kiến trúc đám mây.

### Bài Học Rút Ra
*   Trong các kiến trúc hệ thống hiện đại, việc ứng dụng AI (như Multi-agent) không chỉ giúp tăng tốc độ xử lý mà còn phải được thiết kế để phân quyền rõ ràng, giảm thiểu rủi ro sai lệch dữ liệu.
*   Bảo mật cấp doanh nghiệp luôn đi kèm với bài toán chi phí. Việc lựa chọn công nghệ (như MCP qua Private Link) cần được tính toán kỹ lưỡng dựa trên giá trị cốt lõi và giới hạn ngân sách của dự án.

---
### Một Số Hình Ảnh Khi Tham Gia Sự Kiện

![Hình ảnh tham gia sự kiện 1](/images/4-Event/event-27-6.avif) 

![Hình ảnh tham gia sự kiện 2](/images/4-Event/event-27-6_minhchung.avif)