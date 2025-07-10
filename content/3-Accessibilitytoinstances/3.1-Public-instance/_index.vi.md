---
title : "Tạo Bucket mới trên Amazon S3"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 3.1. </b> "
---
**Tổng quan**: 
Amazon Simple Storage Service (Amazon S3) là một dịch vụ lưu trữ dạng đối tượng cung cấp khả năng mở rộng theo yêu cầu sử dụng, đảm bảo tính khả dụng của dữ liệu, độ bảo mật, và hiệu năng ở mức cao nhất.

S3 được xây dựng để đáp ứng yêu cầu của khách hàng thuộc mọi quy mô và ngành nghề, đều có thể dùng dịch vụ này để lưu trữ và bảo vệ bất kỳ lượng dữ liệu nào.

S3 có thể được dùng cho nhiều trường hợp sử dụng như kho dữ liệu (data warehouse), trang web, ứng dụng di động, sao lưu và khôi phục, lưu trữ, ứng dụng doanh nghiệp, thiết bị IoT và phân tích dữ liệu lớn. Ngoài ra, Amazon S3 còn cung cấp các tính năng quản lý dễ sử dụng, giúp bạn có thể tổ chức dữ liệu và cấu hình các biện pháp kiểm soát truy cập để đáp ứng yêu cầu cụ thể của doanh nghiệp, tổ chức và yêu cầu về tuân thủ.

Amazon S3 được thiết kế để đảm bảo độ bền 99,999999999% (11 9’s) và lưu trữ dữ liệu của hàng triệu ứng dụng cho các công ty trên toàn thế giới.

![SSMPublicinstance](/images/S3.png)

1. Đầu tiên, chúng ta sẽ tạo một S3 bucket:

- Truy cập AWS Management Console.
- Tìm S3.
- Chọn S3.

![Connect](/images/3.connect/001-connect.png)

2. Trong giao diện **S3**, chọn **Create bucket**.
  
  ![Connect](/images/3.connect/002-connect.png)


3. Trong giao diện Create bucket:

- Bucket name: nhập ```aws-first-cloud-journey```.
- AWS Region: chọn region bạn muốn.
- Đối với Object Ownership, chọn ACLs disabled (recommended).

![Connect](/images/3.connect/003-connect.png)
**Lưu ý**: Vì **Bucket name** là duy nhất trên mức độ toàn cầu, nếu sử dụng tên giống như trên sẽ xuất hiện thông báo **“Bucket with the same name already exists”**. Do đó, cần thêm vài số phía sau để **Bucket name** của bạn phù hợp với policy.

![Connect](/images/3.connect/004-connect.png)

4. Bỏ chọn **"Block all public access"** trong phần **Object Ownership & Permissions**

![Connect](/images/3.connect/005-connect.png)

5. Nhấn **Create bucket** để khởi tạo.

![Connect](/images/3.connect/006-connect.png) 

