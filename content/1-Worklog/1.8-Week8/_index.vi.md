---
title: "Worklog Tuần 8"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Ôn tập lại nền tảng cơ sở dữ liệu (Database) và làm quen với các dịch vụ lưu trữ dữ liệu trên mây của AWS như RDS, Aurora, Redshift và ElastiCache.
* Thực hành triển khai ứng dụng kết nối với Database và học cách di chuyển toàn bộ dữ liệu từ nơi này sang nơi khác bằng AWS DMS

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết:** <br>&emsp; + Ôn tập các khái niệm cốt lõi về cơ sở dữ liệu. <br>&emsp; + Tìm hiểu Amazon RDS và kiến trúc của Amazon Aurora.                                                                        | 08/06/2026   | 08/06/2026      |[Video lý thuyết](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217)|
| 3   | - **Học lý thuyết:** <br>&emsp; + Nghiên cứu các giải pháp dữ liệu chuyên biệt: Amazon Redshift (kho dữ liệu khổng lồ) và ElastiCache (cơ chế cache giúp tăng tốc độ đọc dữ liệu cho web).                                         | 09/06/2026   | 09/06/2026      | [Video lý thuyết](https://www.youtube.com/watch?v=UvdiRW34aNI&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=219)|
| 4   | - **Thực hành:** <br>&emsp; + Chuẩn bị hạ tầng: Create EC2 instance và Create RDS database instance. <br>&emsp; + Application Deployment (cài app và kết nối DB). <br>&emsp; + Thử nghiệm Backup and Restore.                       | 10/06/2026   | 10/06/2026      | <https://000005.awsstudygroup.com/>         |
| 5   | - **Thực hành:** <br>&emsp; + Làm quen công cụ AWS DMS. <br>&emsp; + Cấu hình đầu vào/đầu ra: Select your DMS source & Select your DMS Target. <br>&emsp; + Khởi chạy Serverless replication để copy data.                         | 11/06/2026   | 11/06/2026      | <https://000043.awsstudygroup.com/>         |
| 6   | - **Thực hành:** <br>&emsp; + Monitoring DMS Migrations (theo dõi quá trình chuyển data). <br>&emsp; + Troubleshooting Migrations (tập debug và xử lý khi bị lỗi). <br>&emsp; + Clean up resources & Environment Cleanup.       | 12/06/2026   | 12/06/2026      | <https://000043.awsstudygroup.com/>         |


### Kết quả đạt được tuần 8:

* **Hệ quản trị CSDL quan hệ (RDS):** Hiểu rõ cách AWS vận hành cơ sở dữ liệu. Nhờ kiến thức này, em đã biết cách khởi tạo một cụm Amazon RDS MySQL chuẩn chỉnh, cấu hình Security Group nghiêm ngặt để chuẩn bị sẵn sàng cho việc kết nối với các API Backend sau này.
* **Tối ưu tốc độ & Phân tích (ElastiCache & Redshift):** Mở rộng tư duy về cách các hệ thống lớn xử lý hàng triệu lượt truy cập thông qua bộ nhớ đệm (Cache) và cách lưu trữ dữ liệu để phục vụ cho việc phân tích, thống kê (Data Warehouse).
* **Thực chiến triển khai App (Lab 05):** Hoàn thành vòng lặp thực tế của một Backend Developer: Dựng máy chủ (EC2), dựng Database (RDS), đẩy code ứng dụng lên (Application Deployment) và kết nối chúng lại với nhau. Thêm vào đó là việc tự tay test tính năng Backup and Restore để đảm bảo dữ liệu không bị bay màu khi có sự cố.
* **Dịch chuyển dữ liệu (Lab 43):** Làm chủ được kỹ năng "chuyển nhà" cho Database bằng AWS DMS. Biết cách thiết lập trạm nguồn (Source), trạm đích (Target) và đặc biệt là cách đọc log (Monitoring & Troubleshooting) để tìm ra nguyên nhân gốc rễ nếu quá trình chuyển dữ liệu bị gián đoạn.


