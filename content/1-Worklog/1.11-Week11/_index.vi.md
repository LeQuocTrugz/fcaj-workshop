---
title: "Worklog Tuần 11"
date: 2026-07-08
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Đưa toàn bộ dự án Đặt sân bóng đá từ môi trường phát triển (Local) lên môi trường thực tế trên hệ sinh thái AWS.
* Thiết lập tên miền riêng (Custom Domain) để ứng dụng có địa chỉ truy cập chuyên nghiệp.
* Thực hiện kiểm thử toàn trình (End-to-End Test), đánh giá mức độ ổn định và chốt phiên bản đồ án cuối cùng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Dựng hạ tầng AWS thực tế:** <br>&emsp; + Tạo máy chủ ảo EC2 đặt ở Public Subnet. <br>&emsp; + Khởi tạo RDS MySQL đặt ở Private Subnet để bảo vệ dữ liệu. <br>&emsp; + Đảm bảo S3 Bucket đã sẵn sàng lưu ảnh.                      | 29/06/2026   | 29/06/2026      |
| 3   | - **Cấu hình môi trường EC2:** <br>&emsp; + Dùng SSH kết nối vào server Linux, cài đặt Java (Amazon Corretto/JDK). <br>&emsp; + Khai báo các biến môi trường (FB_KEY, GG_KEY, DB_URL, DB_PASS) vào file cấu hình của hệ điều hành.  | 30/06/2026   | 30/06/2026      |
| 4   | -- **Deploy mã nguồn lên AWS:** <br>&emsp; + Thực hiện đưa file đóng gói `.jar` của toàn bộ dự án web lên máy chủ EC2. <br>&emsp; + Cấu hình cho ứng dụng web hoạt động ổn định dưới dạng một tiến trình chạy ngầm. | 01/07/2026       | 01/07/2026      |
| 5   | - **Cấu hình Mạng & Tên miền (Domain):** <br>&emsp; + Hoàn thiện cấu hình Tường lửa (Security Group) cho EC2 và RDS. <br>&emsp; + Đăng ký tên miền riêng và thiết lập bản ghi DNS trỏ thành công về địa chỉ Public IP của EC2.       | 02/07/2026   | 02/07/2026      |
| 6   | - **Kiểm thử & Chốt đồ án:** <br>&emsp; + Truy cập hệ thống qua tên miền chính thức, thực hiện kiểm thử UAT cho toàn bộ luồng nghiệp vụ (Đăng nhập, Đặt sân, Upload ảnh). <br>&emsp; + Theo dõi log hệ thống và chốt đồ án.           | 03/07/2026   | 03/07/2026      |


### Kết quả đạt được tuần 11:

* **Triển khai thành công trên môi trường thực tế:** Hoàn tất việc đưa dự án Spring Boot MVC lên nền tảng đám mây AWS. Ứng dụng hoạt động ổn định, trơn tru 24/7 trên máy chủ Linux mà không gặp gián đoạn.
* **Tích hợp Tên miền chuyên nghiệp:** Thay vì phải truy cập bằng một dải địa chỉ IP khó nhớ, hệ thống đã được gắn tên miền (Domain) chính thức, mang lại trải nghiệm người dùng chuyên nghiệp và hoàn thiện hệt như một sản phẩm thương mại thực thụ.
* **Đảm bảo bảo mật & Kết nối:** Các thành phần của hệ thống giao tiếp an toàn (EC2 kết nối đúng vào private RDS và S3). Toàn bộ các khóa bảo mật (Client Key) được quản lý chặt chẽ ở cấp độ hệ điều hành, không bị rò rỉ trong mã nguồn.
* **Hoàn thiện dự án:** Vượt qua các bước kiểm thử cuối cùng trên môi trường Production, chính thức chốt hạ đồ án kết thúc khóa học Workforce Bootcamp đúng tiến độ đề ra.

