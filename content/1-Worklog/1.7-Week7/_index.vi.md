---
title: "Worklog Tuần 7"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Hiểu rõ ranh giới "ai chịu trách nhiệm gì" khi đưa hệ thống lên mây (Mô hình trách nhiệm chung).
* Nắm bắt các công cụ quản lý tài khoản, phân quyền người dùng (IAM, Cognito) và cách khóa chặt dữ liệu bằng mã hóa.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết (Module 05):** <br>&emsp; + Tìm hiểu "Mô hình trách nhiệm chung" (hiểu đơn giản là AWS bảo vệ hạ tầng vật lý, còn mình tự lo bảo vệ dữ liệu và code của mình)                                                            |1/06/2026   | 1/06/2026      |[Video lý thuyết](https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150)|
| 3   | - **Học lý thuyết:** Các dịch vụ quản lý truy cập <br>&emsp; + Phân biệt IAM, AWS Organization và Identity Center <br>&emsp; + Tìm hiểu Amazon Cognito (cơ chế đăng nhập giống như "Login with Google")                                | 2/06/2026   | 2/06/2026      | [Video lý thuyết](https://www.youtube.com/watch?v=N_vlJGAqZxo&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=151)|
| 4   | - **Khám phá KMS & Thực hành:** <br>&emsp; + Bật dịch vụ Enable Security Hub để giám sát an ninh. <br>&emsp; + Kiểm tra Security Standards và chấm điểm Security Score by Standards. <br>&emsp; + Dọn dẹp tài nguyên                       | 3/06/2026   | 3/06/2026      | <https://000018.awsstudygroup.com/> |
| 5   | - **Thực hành:** <br>&emsp; + Chuẩn bị hạ tầng: Create VPC, Security Group, EC2 instance và cài Incoming Web-hooks slack. <br>&emsp; + Tạo Tag, gán Role cho Lambda, viết Lambda Function và Check Result. <br>&emsp; + Clean up resources. | 4/06/2026   | 4/06/2026      | <https://000022.awsstudygroup.com/> |
| 6   |- **Thực hành:** <br>&emsp; + Sử dụng tag trên Console: Create EC2 Instance with tag, quản lý và Filter resources by tag. <br>&emsp; + Thử nghiệm Using tags with CLI và Create a Resource Group. <br>&emsp; + Clean up resources.                                                                              | 5/06/2026   | 5/06/2026      | <https://000027.awsstudygroup.com/> |


### Kết quả đạt được tuần 7:

* * **Tư duy bảo mật đám mây:** Nắm được luật chơi của "Mô hình trách nhiệm chung", không còn tư duy ỷ lại rằng đưa lên mây là hệ thống tự động an toàn 100%.
* **Giám sát an ninh:** Lần đầu tự tay kích hoạt Security Hub để dò quét lỗ hổng. Biết cách xem báo cáo Security Standards và đánh giá rủi ro qua điểm số Security Score by Standards. Không quên bước Clean Up Resources để tránh phát sinh cước.
* **Tự động hóa & Cảnh báo:** Hoàn thành một luồng (flow) rất thực tế của kỹ sư Cloud: Tự dựng VPC, EC2, sau đó cấu hình Incoming Web-hooks slack. Hiểu được cách tạo Role cấp quyền cho Lambda Function chạy ngầm để bắn thông báo thành công về kênh chat (Check Result). Cuối cùng là Clean up resources.
* **Quản lý tài nguyên:** Nhận ra tầm quan trọng của việc dán nhãn (Tagging) khi hệ thống có quá nhiều máy chủ. Thành thạo việc tạo EC2 Instance with tag, Filter resources by tag trên cả giao diện Console lẫn dòng lệnh CLI. Nắm được cách gom cụm tài nguyên bằng Create a Resource Group và thao tác Clean up resources gọn gàng.


