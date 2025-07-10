---
title : "Website Tĩnh tích hợp Gửi Email bằng AWS Serverless"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
---
# Tạo Website Tĩnh tích hợp Gửi Email bằng AWS Serverless

### Tổng quan

 Trong bài lab này, bạn sẽ tìm hiểu cách triển khai 1 website tĩnh (HTML/CSS) chứa form liên hệ, upload lên AWS S3, kết nối form với AWS Lambda và API Gateway, và sử dụng Amazon SES để gửi email khi người dùng điền form.

![fwd](/images/sodoo.png)

### Nội dung

 1. [Giới thiệu](1-introduce/)
 2. [Các bước chuẩn bị](2-Prerequiste/)
 3. [Triển khai website tĩnh lên S3](3-Accessibilitytoinstance/)
 4. [Tạo Lambda Function xử lý gửi email](4-s3log/)
 5. [Tạo API Gateway để kết nối frontend](5-Portfwd/)
 6. [Dọn dẹp tài nguyên](6-cleanup/)
