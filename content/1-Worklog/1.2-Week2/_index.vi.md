---
title: "Worklog Tuần 2"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Nắm vững lý thuyết về các dịch vụ cốt lõi của AWS bao gồm: Quản lý định danh và truy cập (IAM), Máy chủ ảo đám mây (Amazon EC2) và Dịch vụ lưu trữ khối - ổ cứng ảo (Amazon EBS).
* Áp dụng kiến thức lý thuyết vào các bài thực hành (Lab) để tự tay khởi tạo và cấu hình tài nguyên trên AWS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết:** Nghiên cứu các video bài giảng về Quản lý định danh và truy cập (IAM) <br>&emsp; + Các khái niệm Users, Groups, Roles, Policies <br>&emsp; + Best practices bảo mật                                                             | 27/04/2026   | 27/04/2026      | <https://000002.awsstudygroup.com/> |
| 3   | - **Thực hành:** <br>&emsp; + Thực hành tạo tài khoản IAM User <br>&emsp; + Phân quyền (gán Policy) và thiết lập mật khẩu, MFA cho IAM User an toàn                                                                                            | 28/04/2026   | 28/04/2026      | <https://000002.awsstudygroup.com/2-create-admin-user-and-group/> |
| 4   |- **Học lý thuyết:** Nghiên cứu video bài giảng về Máy chủ ảo (Amazon EC2) và Ổ cứng ảo (Amazon EBS) <br>&emsp; + Các loại Instance Types <br>&emsp; + Cơ chế hoạt động của EBS                                                                      | 29/04/2026   | 29/04/2026      | <https://000004.awsstudygroup.com/> |
| 5   | - **Thực hành:** <br>&emsp; + Khởi tạo và thiết lập máy chủ ảo EC2 (chọn AMI, Instance Type, Key Pair) <br>&emsp; + Chạy thử máy chủ và kiểm tra kết nối SSH/SSM                                                                                     | 30/04/2026   | 30/04/2026      | <https://000003.awsstudygroup.com/4-createec2server/> |
| 6   | - **Thực hành:** <br>&emsp; + Thực hiện tạo mới một ổ cứng ảo (EBS volume) <br>&emsp; + Gắn (attach) ổ cứng vào máy chủ EC2 đang hoạt động <br>&emsp; + Định dạng ổ cứng trong OS                                                               | 01/05/2026   | 01/05/2026      | <https://000003.awsstudygroup.com/4-createec2server/> |


### Kết quả đạt được tuần 2:

* Nắm vững cơ chế bảo mật và quản lý phân quyền của AWS thông qua dịch vụ IAM.
* Khởi tạo và cấu hình thành công các IAM User, phân quyền đúng chuẩn nguyên tắc "Đặc quyền tối thiểu" (Least Privilege).
* Hiểu rõ khái niệm và vòng đời hoạt động của một máy chủ ảo trên đám mây (Amazon EC2).
* Tự tay khởi tạo, thiết lập mạng, bảo mật (Security Groups) và kết nối thành công vào máy chủ EC2.
* Nắm bắt được cách thức mở rộng không gian lưu trữ cho máy chủ bằng cách tạo mới, gắn thêm và định dạng thành công ổ cứng ảo (EBS volume) ngay khi máy chủ đang hoạt động.


