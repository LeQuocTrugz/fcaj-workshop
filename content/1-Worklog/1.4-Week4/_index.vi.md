---
title: "Worklog Tuần 4"
date: 2026-07-08
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Làm chủ các khái niệm bảo mật mạng nhiều lớp trên AWS (Security Group, Network ACLs) và công cụ trực quan hóa mạng VPC Resource Map.
* Thực hành xây dựng một hệ thống mạng đám mây tùy chỉnh (Custom VPC) hoàn chỉnh từ con số 0, bao gồm cấu hình định tuyến, giám sát lưu lượng và thiết lập truy cập từ xa an toàn.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Học lý thuyết:** Tìm hiểu sâu về bảo mật mạng AWS <br>&emsp; + Phân biệt Security Group (Stateful) và Network ACLs (Stateless) <br>&emsp; + Đọc hiểu sơ đồ mạng qua VPC Resource Map                                                        | 11/05/2026   | 11/05/2026      |[Video lý thuyết](https://www.youtube.com/watch?v=BPuD1l2hEQ4&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=26) |
| 3   | - **Thực hành (Lab):** Xây dựng hạ tầng mạng cơ bản <br>&emsp; + Khởi tạo Custom VPC <br>&emsp; + Chia Subnet (Public và Private) <br>&emsp; + Gắn Internet Gateway và cấu hình Route Table                                                    | 12/05/2026   | 12/05/2026      | <https://000003.awsstudygroup.com/> |
| 4   |- **Thực hành (Lab):** Thiết lập bảo mật & Giám sát mạng <br>&emsp; + Tạo và gắn Security Group cho các tài nguyên <br>&emsp; + Kích hoạt VPC Flow Logs để lưu vết lưu lượng mạng (Traffic)                                                    | 13/05/2026   | 13/05/2026      | <https://000003.awsstudygroup.com/> |
| 5   | - **Thực hành (Lab):** Giao tiếp ngoại mạng (Outbound) <br>&emsp; + Triển khai EC2 vào mạng vừa tạo <br>&emsp; + Cấu hình NAT Gateway <br>&emsp; + Kiểm tra kết nối bằng Reachability Analyzer                                                 | 14/05/2026   | 15/05/2026      | <https://000003.awsstudygroup.com/> |
| 6   | - **Thực hành (Lab):** Thiết lập truy cập từ xa <br>&emsp; + Cấu hình EC2 Instance Connect Endpoint (EICE) <br>&emsp; + Thử nghiệm kết nối SSH an toàn vào Private EC2 không cần Public IP                                                    | 15/05/2026   | 15/05/2026      | <https://000003.awsstudygroup.com/> |


### Kết quả đạt được tuần 4:

* **Bảo mật & Giám sát mạng (Network Security & Monitoring):** Nắm được sự khác biệt và cách kết hợp giữa Security Group và Network ACLs. Kích hoạt thành công VPC Flow Logs để theo dõi luồng dữ liệu và sử dụng VPC Resource Map để trực quan hóa kiến trúc.
* **Triển khai hạ tầng mạng cơ sở (VPC & Routing):** Tự tay phác thảo và cấu hình thành công một môi trường mạng hoàn chỉnh bao gồm VPC, chia tách Public/Private Subnets, Internet Gateway và bảng định tuyến (Route Tables).
* **Giao tiếp ngoại mạng an toàn (NAT Gateway):** Triển khai NAT Gateway giúp các máy chủ ảo (EC2) nằm trong vùng Private Subnet có thể truy cập internet an toàn để cập nhật phần mềm; ứng dụng Reachability Analyzer để kiểm thử và gỡ lỗi luồng mạng.
* **Truy cập từ xa bảo mật (Remote Access):** Thiết lập thành công EC2 Instance Connect Endpoint, tạo ra một đường hầm bảo mật cho phép kết nối (SSH) trực tiếp vào máy chủ ảo trong mạng nội bộ mà không cần phải mở cổng hay gán Public IP ra ngoài Internet.


