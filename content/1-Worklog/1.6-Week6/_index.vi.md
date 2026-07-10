---
title: "Worklog Tuần 6"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:
* Biết cách lưu trữ trên mây với Amazon S3, từ việc host một trang web tĩnh cơ bản đến các trò nâng cao như chống xóa nhầm và nhân bản dữ liệu xuyên quốc gia.
* Biết cách gắn mạng phân phối nội dung (CloudFront) để web load nhanh ở mọi nơi và tìm hiểu các giải pháp chuyển lượng dữ liệu khổng lồ lên mây.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết:** Xem video Module 04 về hệ sinh thái lưu trữ AWS <br>&emsp; + Cách quản lý quyền truy cập S3 ai được xem, ai bị cấm <br>&emsp; + Tìm hiểu quy tắc CORS                                                                               | 11/08/2025   | 11/08/2025      |[Video lý thuyết](https://www.youtube.com/watch?v=_yunukwcAwc&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=104)|
| 3   | - **Thực hành:** Chạy website không cần server <br>&emsp; + Tạo S3 Bucket, up source code web tĩnh (HTML/CSS/JS) lên <br>&emsp; + Cấu hình public access để ai cũng vào xem web được                                                                  | 12/08/2025   | 12/08/2025      | <https://000057.awsstudygroup.com/> |
| 4   | - **Thực hành:** Tăng tốc web bằng CDN <br>&emsp; + Tích hợp Amazon CloudFront vào web S3 vừa tạo <br>&emsp; + Chặn truy cập thẳng vào S3, bắt buộc người dùng phải đi qua CloudFront                                                                   | 13/08/2025   | 13/08/2025      | <https://000057.awsstudygroup.com/> |
| 5   | - **Thực hành:** Tính năng S3 nâng cao <br>&emsp; + Bật Versioning (lưu lại các phiên bản cũ) để lỡ xóa nhầm còn cứu được <br>&emsp; + Cấu hình tự động nhân bản data sang Region khác (CRR)                                                           | 14/08/2025   | 15/08/2025      | <https://000057.awsstudygroup.com//> |
| 6   | -- **Học lý thuyết:** Các cách vận chuyển data <br>&emsp; + Mở mang tầm mắt với thiết bị nhà Snow (Snowcone, Snowball, Snowmobile) <br>&emsp; + Ôn lại Storage Gateway và AWS Backup                                                                   | 15/08/2025   | 15/08/2025      | [Video lý thuyết](https://www.youtube.com/watch?v=YXn8Q_Hpsu4&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=106)|


### Kết quả đạt được tuần 6:
* **Host web tĩnh (Amazon S3):** Tự tay đưa được một trang web tĩnh lên mạng Internet chạy mượt mà chỉ bằng S3 mà không cần tốn tiền thuê nguyên cái máy chủ (server).
* **Tăng tốc & Bảo mật (CloudFront):** Biết cách giấu kín bucket S3 ở phía sau, tích hợp CloudFront làm mạng phân phối nội dung (CDN) giúp web load nhanh hơn nhờ cơ chế cache và chống bị ddos tấn công trực tiếp.
* **Bảo vệ file an toàn (S3 Nâng cao):** Mở khóa được tính năng "thần thánh" Versioning giúp khôi phục file lỡ tay ghi đè/xóa nhầm. Đồng thời biết cách cấu hình Cross-Region Replication để tự động dự phòng dữ liệu sang tận đầu bên kia quả địa cầu.
* **Di chuyển dữ liệu (Data Migration):** Nắm được các giải pháp bê nguyên một trung tâm dữ liệu khổng lồ lên mây bằng các thiết bị vật lý chuyên dụng (Snow Family) thay vì phải ngồi upload qua mạng internet thông thường.


