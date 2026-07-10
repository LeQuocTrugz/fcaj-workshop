---
title: "Worklog Tuần 9"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Lên ý tưởng, thảo luận cùng nhómr và chốt đề tài dự án thực tập tổng kết khóa học.
* Phân tích các yêu cầu, phác thảo sơ đồ kiến trúc hệ thống trên **draw.io** và tiến hành review, thảo luận cùng Mentor và chỉnh sửa để ra được bản thiết kế tối ưu nhất.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Lên ý tưởng đề tài:** <br>&emsp; + Brainstorming các chủ đề khả thi. <br>&emsp; + Thảo luận với nhóm và chính thức chốt đề tài: **Xây dựng Hệ thống quản lý đặt sân bóng đá**.                                                 | 15/06/2026   | 15/06/2026      |
| 3   |- **Phân tích yêu cầu:** <br>&emsp; + Liệt kê các tính năng cốt lõi (Tìm sân, đặt lịch, thanh toán, quản lý user). <br>&emsp; + Thiết kế sơ bộ lược đồ Cơ sở dữ liệu (Database Schema) cho hệ thống.                                 | 16/06/2026   | 16/06/2026      | 
| 4   | - **Thiết kế kiến trúc AWS (Bản nháp 1):** <br>&emsp; + Vận dụng kiến thức đã học để vẽ luồng hệ thống. <br>&emsp; + Thảo luận với nhóm để biết lỗi sai cần sửa                                                                      | 17/06/2026   | 17/06/2026      | Draw.io |
| 5   | - **Review & Gỡ lỗi thiết kế:** <br>&emsp; + Trình bày sơ đồ nháp với Mentor và team. <br>&emsp; + **Phát hiện lỗi:** Đặt sai luồng bảo mật của Database và thiếu các cổng kết nối (Endpoint) nội bộ an toàn.                    | 18/06/2026   | 18/06/2026      |  
| 6   | - **Chốt kiến trúc tổng thể:** <br>&emsp; + Sửa lại sơ đồ: Bổ sung S3 Gateway Endpoint và RDS Endpoint. <br>&emsp; + Cập nhật cơ chế Multi-AZ cho Database. <br>&emsp; + Hoàn thiện bản vẽ kiến trúc AWS cuối cùng.    | 19/06/2026   | 19/06/2026      | Draw.io   |

### Kết quả đạt được tuần 9:
* **Chốt chặn đề tài:** Xác định rõ ràng mục tiêu và phạm vi của dự án "Hệ thống đặt sân bóng đá", tạo bước đệm vững chắc cho giai đoạn code.
* **Tư duy thiết kế hệ thống:** Trải qua quá trình "vẽ - sai - sửa lại", em đã hiểu sâu sắc hơn lý do tại sao phải dùng Gateway Endpoint thay vì đi vòng ra Internet, và tầm quan trọng của việc đặt Database vào vùng Private Subnet khép kín. Bản sơ đồ kiến trúc AWS cuối cùng đã được Mentor duyệt và sẵn sàng cho việc triển khai thực tế.
