---
title: "Event 1"
date: 2026-07-05
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# BÀI THU HOẠCH: AWS FIRST CLOUD AI JOURNEY – COMMUNITY DAY

### Mục Đích Của Sự Kiện
*   Cập nhật các bước tiến công nghệ mới nhất về Generative AI (GenAI), Large Language Models (LLMs) và kiến trúc Đa tác tử (Multi-Agent).
*   Chia sẻ các phương pháp thiết kế hạ tầng mạng biên vững chắc, bảo mật và tối ưu chi phí bằng Amazon CloudFront.
*   Trao đổi kinh nghiệm thực tế về quy trình phát triển sản phẩm công nghệ từ ý tưởng đến thực thi dưới áp lực thời gian lớn (Hackathon).
*   Định hướng nghề nghiệp và xây dựng tư duy ứng dụng AI thực tế cho cộng đồng công nghệ và sinh viên kỹ thuật.

### Danh Sách Diễn Giả
*   **Tinh Truong** - Platform Engineer, GoTymeX
*   **Anh Pham** - Cloud Consultant, G-AsiaPacific Vietnam
*   **Thinh Nguyen** - DevOps Engineer, FCAJ
*   **Team VIB** (Thao Nguyen, Mai Nguyen, Uyen Le) 
*   **Duc Dao** - Solutions Architect, Cloud Kinetics
*   **Vy Lam** - Senior Business Systems Analyst - VPBank

---

### Nội Dung Nổi Bật

#### 1. Context Is Everything: Making AI Actually Work for You
*   **Lý do AI thất bại:** AI thường không mang lại kết quả như kỳ vọng nếu thiếu bối cảnh (context) cụ thể. Bản chất của sự tiến hóa AI là dịch chuyển từ các câu lệnh Prompt đơn thuần sang hệ thống ghi nhớ nâng cao (khái niệm "Second AI Brain").
*   **Giải pháp nâng cao bối cảnh:** Việc cung cấp ngữ cảnh tốt hơn sẽ tối ưu hóa chất lượng đầu ra. Bài tham luận cũng mở ra các góc nhìn nghề nghiệp thực tế về cách sinh viên có thể bắt đầu xây dựng dự án với AI.

#### 2. Friendly AI Assistant with Amazon Quick
Giới thiệu bộ giải pháp hỗ trợ thông minh dựa trên Amazon Quick giúp đơn giản hóa tương tác dữ liệu:
*   **Quick Chat Agent & Spaces:** Trợ lý AI hỗ trợ khám phá, phân tích dữ liệu và không gian cộng tác chia sẻ tri thức cá nhân thành tri thức đội ngũ.
*   **Quick Flows & Sight:** Cho phép tạo các luồng công việc thông minh (intelligent workflows) và xây dựng dashboard/report trực quan từ dữ liệu thô hoàn toàn bằng ngôn ngữ tự nhiên mà không cần viết code.

#### 3. From Edge To Origin: CloudFront as Your Foundation
*   **Hạ tầng nền tảng:** Vai trò của Amazon CloudFront đối với mọi loại Workload từ tĩnh đến động.
*   **Các trụ cột cốt lõi:** Phân tích chuyên sâu 4 yếu tố trọng tâm: Tối ưu hóa chi phí vận hành băng thông mạng biên, tăng cường các năng lực bảo mật lớp biên, củng cố tính đáng tin cậy (reliability) và nâng cao hiệu năng (performance) tổng thể cho hệ thống từ Edge tới Origin.

#### 4. 36 hrs with LotusHacks – Building UTMorpho from Idea to Reality
*   **Hành trình Hackathon:** Chia sẻ thực tế từ Team VIB về trải nghiệm tham gia LotusHacks. Quá trình động não (brainstorming) từ con số 0 để định hình bài toán và phát triển sản phẩm UTMorpho.
*   **Áp lực thực thi:** Kinh nghiệm chạy sprint công nghệ liên tục trong 36 giờ, cách đối mặt với thách thức, xử lý thất bại tại các điểm nút quan trọng để hoàn thiện bản Demo sản phẩm cuối cùng.

#### 5. Non-Determinism of "Deterministic" LLM Settings
*   **Cơ chế chọn Token:** Đi sâu vào cách các mô hình ngôn ngữ lớn (LLMs) dự đoán và lựa chọn token tiếp theo.
*   **Phản bác giả định kỹ thuật:** Làm rõ thực tế rằng thiết lập `Temperature = 0` không hoàn toàn đảm bảo tính thấu suốt/định tính (determinism) do các kỹ thuật tối ưu hóa quá trình suy luận (inference optimizations) tác động, từ đó đề xuất các chiến lược giảm thiểu rủi ro trong ứng dụng thực tế.

#### 6. Enterprise-Grade Multi-Agent System: Credit Scoring
*   **Bài toán doanh nghiệp:** Sự lệch pha về mặt cấu trúc giữa dữ liệu của các startup với hệ thống Core Banking truyền thống khi chấm điểm tín dụng.
*   **Mô hình Multi-Agent:** Đánh giá khi nào nên và không nên dùng Single Agent. Đưa ra kiến trúc mẫu cho một "Hội đồng tín dụng ảo" (Virtual Credit Committee) tích hợp các bộ quy tắc kiểm soát hành vi (Guardrails), tuân thủ pháp lý cùng lộ trình FinOps/ROI khi triển khai thực tế.

---

### Những Gì Học Được

#### Tư Duy Thiết Kế
*   **Context-Driven Mindset:** Hiểu rõ tầm quan trọng của ngữ cảnh (Context) trong việc vận hành Generative AI, giúp hạn chế hiện tượng ảo tưởng (hallucination) của mô hình.
*   **Multi-Agent Paradigm:** Tư duy chia nhỏ bài toán phức tạp thành nhiều tác tử chuyên biệt làm việc cùng nhau giúp giải quyết các nghiệp vụ lớn đòi hỏi tính tuân thủ cao của doanh nghiệp.

#### Kiến Trúc Kỹ Thuật
*   **Hạ tầng Cloud-native biên:** Nắm vững cách thiết lập Amazon CloudFront làm lớp khiên bảo mật và tăng tốc hiệu năng cho backend nguồn (Origin).
*   **Sự bất định của LLM:** Nhận thức rõ bản chất bất định (Non-determinism) của LLM để không phụ thuộc mù quáng vào các thiết lập tham số, chuẩn bị sẵn các giải pháp bọc mã nguồn chống lỗi ở tầng ứng dụng.

---

### Ứng Dụng Vào Công Việc & Đồ Án
*   **Tối ưu hóa Deployment Đồ án:** Áp dụng kiến trúc CDN biên của CloudFront kết hợp bảo mật Layer 7 để tối ưu tốc độ tải và chống tấn công trực diện vào cụm máy chủ Backend EC2 của Website Đặt Sân Bóng Đá.
*   **Tích hợp AI Contextual:** Ứng dụng kỹ thuật cung cấp ngữ cảnh hệ thống (System Context) khi phát triển các tính năng hỗ trợ thông minh bằng AI chatbot trong tương lai, tránh việc gọi API trả kết quả chung chung.
*   **Kinh nghiệm quản lý dự án dưới áp lực:** Học hỏi tinh thần Sprint 36 giờ từ đội ngũ Hackathon để tối ưu hóa tiến độ làm việc nhóm, phân chia Module độc lập nhằm hoàn thành đồ án đúng hạn.

---

### Trải Nghiệm Trong Sự Kiện
Tham gia sự kiện **AWS First Cloud AI Journey - Community Day** tại tầng 26 là một trải nghiệm công nghệ rất giá trị. Tại đây, tôi có cơ hội:
*   Lắng nghe trực tiếp từ các chuyên gia DevOps, Solutions Architect và GenAI Engineer đến từ các tổ chức uy tín (GoTymeX, Cloud Kinetics, G-AsiaPacific, VPBank, VIB), giúp thu hẹp khoảng cách giữa lý thuyết giảng đường và thực tế doanh nghiệp.
*   Quan sát trực quan các bài Demo thực tế về hệ thống Multi-Agent và sản phẩm UTMorpho, từ đó hiểu được cách kết hợp các dịch vụ Cloud để tạo ra giá trị kinh doanh cụ thể.
*   Kết nối và trao đổi trong phiên Q&A với các diễn giả về các xu hướng công nghệ sẽ bùng nổ trong năm 2026, đặc biệt là xu hướng hạ tầng mạng tự động hóa (NaaS) và ứng dụng không mã nguồn (No-code AI).

### Bài Học Rút Ra
*   Công nghệ AI muốn ứng dụng thành công vào môi trường Enterprise bắt buộc phải đi kèm với hai yếu tố: **Ngữ cảnh (Context)** sâu sắc và **Hệ thống kiểm soát (Guardrails)** chặt chẽ.
*   Hạ tầng đám mây hiện đại luôn phải đặt yếu tố **Bảo mật và Tối ưu chi phí từ gốc tới biên (Edge to Origin)** lên hàng đầu trước khi tính đến chuyện mở rộng quy mô.

---

### Một Số Hình Ảnh Khi Tham Gia Sự Kiện

![Poster Sự kiện AWS Community Day 2026](/fcaj-workshop/images/4-Event/event-23-5.avif)

![Hình ảnh tham gia sự kiện 1](/fcaj-workshop/images/4-Event/hinh_minh_chung_23-5.jpg)