---
title : "Giới thiệu"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**Website tĩnh với xử lý form liên hệ** là một mô hình phổ biến trong việc xây dựng các website đơn giản, nhẹ, dễ triển khai như trang giới thiệu công ty, portfolio cá nhân hay landing page thu thập phản hồi khách hàng.

Trong workshop này, bạn sẽ được hướng dẫn cách triển khai một website tĩnh sử dụng dịch vụ **Amazon S3** để lưu trữ, **CloudFront** để phân phối nội dung toàn cầu và đảm bảo kết nối bảo mật qua HTTPS. Đặc biệt, phần **form liên hệ** sẽ không cần backend truyền thống mà thay vào đó sử dụng kiến trúc **Serverless** gồm:

- **Amazon API Gateway**: định tuyến request từ form
- **AWS Lambda**: xử lý nội dung form
- **Amazon SES**: gửi email thông báo về nội dung liên hệ

 **Bạn sẽ học được cách:**

- Xây dựng website tĩnh và công khai trên S3
- Phân phối nội dung qua CDN (CloudFront) với HTTPS
- Tạo API serverless để xử lý form gửi từ client
- Gửi email tự động qua SES
- Tận dụng hạ tầng cloud không cần máy chủ (serverless)