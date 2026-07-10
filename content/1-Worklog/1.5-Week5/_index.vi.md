---
title: "Worklog Tuần 5"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Tìm hiểu kỹ hơn về cách hoạt động của máy chủ ảo EC2 và cách hệ thống tự động thêm bớt máy chủ khi lượng người dùng thay đổi.
* Biết cách cài đặt tính năng tự động sao lưu dữ liệu (backup) để phòng ngừa rủi ro và cách kết nối ổ cứng trên mây.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết:** Xem video bài giảng (Module 03) về dịch vụ máy chủ EC2 <br>&emsp; + Hiểu cách chọn loại máy chủ (CPU, RAM) sao cho phù hợp và tiết kiệm chi phí                                                                 | 11/08/2025   | 11/08/2025      |[Video lý thuyết](https://www.youtube.com/watch?v=e7XeKdOVq40&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=73)|
| 3   | - **Học lý thuyết:** Tìm hiểu các tính năng nâng cao <br>&emsp; + Cơ chế Auto Scaling (giúp web không bị sập khi có lượng lớn người truy cập) <br>&emsp; + Các loại ổ cứng mạng EFS/FSx                                              | 12/08/2025   | 12/08/2025      | [Video lý thuyết](https://www.youtube.com/watch?v=bbLcPitXJSY&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=79)|
| 4   |- **Thực hành:** Tập làm quen với AWS Backup <br>&emsp; + Tự tay cài đặt lịch sao lưu dữ liệu tự động cho hệ thống thay vì phải copy thủ công                                                                              | 13/08/2025   | 13/08/2025      | <https://000013.awsstudygroup.com/> |
| 5   |- **Thực hành:** <br>&emsp; + Chạy thử tính năng khôi phục (Test Restore) xem bản backup có bị lỗi không, sau đó xóa đi để tránh mất tiền oan.                                                                              | 14/08/2025   | 15/08/2025      | <https://000013.awsstudygroup.com/> |
| 6   | - **Thực hành:** Cấu hình Storage Gateway <br>&emsp; + Dùng một máy EC2 làm "trạm trung chuyển" để đồng bộ file trực tiếp lên kho lưu trữ đám mây S3                                                                                       | 15/08/2025   | 15/08/2025      | <https://000024.awsstudygroup.com/> |


### Kết quả đạt được tuần 5:

* **Quản lý máy chủ:** Đã hiểu cách vận hành và biết cách thiết lập để máy chủ ảo trên AWS tự động nhân bản lên khi hệ thống bị quá tải.
* **Bảo vệ dữ liệu:** Không chỉ biết cách backup dữ liệu tự động mà còn tự tay thử nghiệm khôi phục lại (restore) thành công để đảm bảo hệ thống luôn an toàn nếu xảy ra sự cố.
* **Lưu trữ thực tế:** Nắm được cách đồng bộ file từ máy chủ ở dưới (local) lên thẳng không gian lưu trữ đám mây (S3) một cách mượt mà thông qua Storage Gateway.


