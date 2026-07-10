---
title: "Worklog Tuần 10"
date: 2026-07-08
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Hoàn thiện mã nguồn ứng dụng web Đặt sân bóng đá theo kiến trúc Spring Boot
* Tích hợp đăng nhập mạng xã hội và xử lý bảo mật cho các file cấu hình (giấu các biến nhạy cảm như Client Key Facebook/Google, mật khẩu DB).
* Đóng gói toàn bộ mã nguồn thành một file `.jar` duy nhất để chuẩn bị deploy.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Xây dựng giao diện (View):** <br>&emsp; + Khởi tạo cấu trúc dự án Spring Boot MVC, tích hợp Template Engine (Thymeleaf) và Bootstrap. <br>&emsp; + Dựng khung Layout chuẩn cho web (Header, Footer, Menu) và trang chủ.                                     | 22/06/2026   | 22/06/2026      |
| 3   | - **Xử lý logic (Controller & Model):** <br>&emsp; + Code các chức năng cốt lõi: Đổ danh sách sân bóng ra giao diện, xử lý Form điền thông tin đặt lịch từ người dùng. <br>&emsp; + Map dữ liệu từ HTML Form vào các Entity để lưu xuống DB.                  | 23/06/2026   | 23/06/2026      |
| 4   | - **Bảo mật & Tích hợp Login:** <br>&emsp; + Dùng Spring Security tích hợp luồng đăng nhập bằng Google/Facebook (OAuth2). <br>&emsp; + Tách file `application.properties`, giấu Client Key, Secret Key và mật khẩu DB vào biến môi trường.                  | 24/06/2026   | 24/06/2026      |
| 5   | - **Tích hợp upload ảnh lên AWS S3:** <br>&emsp; + Code chức năng (Controller) nhận file ảnh từ form upload của người dùng (ảnh sân, avatar) và đẩy trực tiếp lên S3 Bucket bằng AWS SDK. <br>&emsp; + Xử lý hiển thị link ảnh S3 ra View.                     | 25/06/2026   | 25/06/2026      |
| 6   | - **Build & Đóng gói dự án:** <br>&emsp; + Sử dụng Maven để build gộp cả code Java và các thư mục tĩnh (HTML, CSS, JS) vào chung một file `.jar`. <br>&emsp; + Chạy thử file `.jar` dưới local bằng command line để test xem web có vỡ giao diện không.      | 26/06/2026   | 26/06/2026      |


### Kết quả đạt được tuần 10:

* **Hoàn thiện ứng dụng:** Xây dựng thành công hệ thống web liền mạch, từ giao diện người dùng (Thymeleaf/Bootstrap) đến logic lưu trữ phía sau đều hoạt động trơn tru trong một project Spring Boot.
* **Bảo mật mã nguồn:** Không còn "hardcode" các thông tin nhạy cảm vào code. Đã biết cách thiết lập để ứng dụng tự động đọc các Key của Facebook, Google và Database từ biến môi trường của hệ điều hành, giúp mã nguồn an toàn khi đẩy lên Github.
* **Đóng gói thành công:** Đóng gói trọn vẹn toàn bộ dự án web thành một file `.jar` duy nhất, không bị lỗi thiếu file giao diện khi chạy thực thi độc lập.


