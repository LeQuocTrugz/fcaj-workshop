---
title: "Event 2"
date: 2026-07-05
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# BÀI THU HOẠCH: AWS COMMUNITY MEETUP (06/06/2026)

### Mục Đích Của Sự Kiện
*   Khám phá các công nghệ Điện toán đám mây tiên tiến, tập trung vào bảo mật, container hóa (containerization) và quản trị cơ sở dữ liệu.
*   Tìm hiểu sự tích hợp giữa Machine Learning và Generative AI (GraphRAG) với hạ tầng AWS.
*   Tiếp cận các kiến trúc đám mây thời gian thực (real-time) dành cho game và ứng dụng tương tác.
*   Phát triển kỹ năng mềm để làm việc nhóm hiệu quả và vạch ra lộ trình chuyển đổi nghề nghiệp rõ ràng sang các vị trí Cloud, DevOps.

### Danh Sách Diễn Giả
*   **Lê Hoàng Gia Đại** - Speaker
*   **Bảo Huỳnh** - Founder and Head of ITea Lab
*   **Nguyễn Quốc Bảo** - Speaker
*   **Trương Phước** - Speaker
*   **Việt Phát** - AI majoring at Swinburne University of Technology
*   **Vinh Trần** - System Administrator at Central Retail Group

---

### Nội Dung Nổi Bật

#### 1. Kết hợp AWS WAF với Machine Learning
*   **Bảo mật không gian mạng:** Khám phá cách Tường lửa ứng dụng web (WAF) dựa trên quy tắc (rule-based) truyền thống có thể được tăng cường bằng Machine Learning để phát hiện và giảm thiểu các cuộc tấn công mạng tinh vi, zero-day trên môi trường AWS.

#### 2. Docker - Công nghệ Container hóa
*   **Khái niệm cốt lõi:** Làm rõ sự khác biệt giữa container hóa và ảo hóa (virtualization). Thảo luận về cách Docker đóng gói ứng dụng và các dependencies thành các đơn vị tiêu chuẩn để phát triển phần mềm, đảm bảo tính nhất quán qua các môi trường máy tính khác nhau.

#### 3. Multiplayer trên Cloud: Godot & AWS WebSockets
*   **Kiến trúc thời gian thực (Real-time):** Trình bày cách xây dựng kiến trúc nhiều người chơi có khả năng mở rộng bằng cách kết nối các client của game engine Godot với AWS WebSockets, làm nổi bật giao tiếp hai chiều, độ trễ thấp trên cloud.

#### 4. AWS Neptune và GraphRAG
*   **Cơ sở dữ liệu nâng cao:** Giới thiệu AWS Neptune như một dịch vụ cơ sở dữ liệu đồ thị (graph database) được quản lý hoàn toàn. Giải thích vai trò quan trọng của nó trong việc xây dựng Graph Knowledge Base để vận hành GraphRAG, giúp cải thiện đáng kể ngữ cảnh và độ chính xác của các ứng dụng Generative AI.

#### 5. Hành trình nghề nghiệp & Làm việc nhóm hiệu quả
*   **Phát triển chuyên môn:** Chia sẻ lộ trình tự học thực tế từ vai trò IT Helpdesk lên Senior Sysadmin và cuối cùng là Cloud/DevOps. Đi kèm với các chiến lược thực tiễn để cải thiện giao tiếp, phân công công việc và cộng tác hiệu quả trong các đội ngũ công nghệ.

---

### Những Gì Học Được

#### Tư Duy Thiết Kế
*   **Tư duy Container-First:** Chuyển dịch từ mô hình triển khai truyền thống sang môi trường container hóa để đảm bảo tính di động của ứng dụng, loại bỏ hoàn toàn vấn đề "code chạy tốt trên máy tôi nhưng lỗi trên server".
*   **Mô hình hóa dữ liệu theo ngữ cảnh:** Hiểu cách cơ sở dữ liệu đồ thị (AWS Neptune) lập bản đồ các mối quan hệ dữ liệu phức tạp hiệu quả hơn so với cơ sở dữ liệu quan hệ truyền thống cho các bài toán AI cụ thể.

#### Kiến Trúc Kỹ Thuật
*   **Tự động hóa bảo mật:** Nắm bắt kiến trúc tích hợp mô hình ML với AWS WAF để tạo ra một tuyến phòng thủ thông minh, tự động cập nhật và bảo vệ các ứng dụng web khỏi rủi ro.
*   **Hướng sự kiện & Thời gian thực:** Hiểu cách triển khai AWS WebSockets để duy trì các kết nối liên tục (persistent connections), điều cực kỳ quan trọng cho các tính năng real-time và đồng bộ hóa.

---

### Ứng Dụng Vào Công Việc & Đồ Án
*   **Tăng cường bảo mật Backend:** Áp dụng các khái niệm về AWS WAF được thảo luận trong sự kiện để thiết lập lớp bảo mật vững chắc cho cụm máy chủ EC2 và cơ sở dữ liệu Amazon RDS của đồ án Website Đặt Sân Bóng Đá, chủ động lọc các lưu lượng web độc hại.
*   **Triển khai Container hóa:** Sử dụng Docker để đóng gói backend Java Spring Boot. Quá trình này sẽ hợp lý hóa luồng triển khai (deployment pipeline), đảm bảo ứng dụng vận hành nhất quán dù đang chạy test ở môi trường local hay mở rộng tự động (auto-scaling) trên AWS.
*   **Phát triển nghề nghiệp & Kỹ năng cộng tác:** Vận dụng các chiến lược làm việc nhóm Agile/Scrum và lộ trình thăng tiến để tăng cường mức độ gắn kết với các thành viên trong dự án. Những góc nhìn này giúp định hình tư duy giải quyết vấn đề và trau dồi năng lực cốt lõi, tạo bước đệm hoàn hảo cho kỳ thực tập tốt nghiệp vị trí Backend Developer sắp tới.

---

### Trải Nghiệm Trong Sự Kiện
Tham gia sự kiện Meetup vào ngày 06/06/2026 là một trải nghiệm công nghệ rất giá trị. Tại đây, tôi có cơ hội:
*   Có được cái nhìn toàn diện về cách các dịch vụ AWS (WAF, WebSockets, Neptune) có thể được phối hợp thiết kế để giải quyết các bài toán kỹ thuật phức tạp và riêng biệt.
*   Lắng nghe những chặng đường nghề nghiệp chân thực, mang lại góc nhìn thực tế về sự cần thiết của việc học tập liên tục để bứt phá trong ngành công nghệ.
*   Tương tác với cộng đồng để thảo luận từ những khái niệm kỹ thuật chuyên sâu (như container hóa) đến những kỹ năng mềm tối quan trọng như nghệ thuật làm việc nhóm.

### Bài Học Rút Ra
*   Bảo mật đám mây hiện đại đòi hỏi nhiều hơn là các bộ quy tắc tĩnh (static rules); việc tích hợp Machine Learning với các công cụ như AWS WAF là bắt buộc để chủ động phát hiện mối đe dọa.
*   Làm chủ các công cụ nền tảng như Docker và am hiểu các mô hình cơ sở dữ liệu đa dạng (như Graph Database) là những kỹ năng sống còn đối với một kỹ sư phát triển phần mềm hiện đại.
*   Năng lực kỹ thuật xuất sắc phải luôn được song hành với khả năng giao tiếp hiệu quả và tinh thần tự học không ngừng nghỉ để tiến xa trên con đường sự nghiệp.

---

### Một Số Hình Ảnh Khi Tham Gia Sự Kiện

![Hình ảnh tham gia sự kiện 1](/images/4-Event/hinh_minh_chung_6-6.jpg) 
