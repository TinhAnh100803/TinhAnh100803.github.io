---
title : "Bật CORS cho Route"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 5.2 </b> "
---

1. Mở **API Gateway** đã tạo, chọn API bạn vừa tạo **contact-form-api**, Vào menu **Routes**

![fwd](/images/5.fwd/012.fwd.png)  

1. Trong phần cột trái, chọn **CORS** 

![fwd](/images/5.fwd/013.fwd.png)  


3. Cấu hình **CORS** : 
  - **Access-Control-Allow-Origin**: *
  - **Access-Control-Allow-Methods**: chọn **POST**, **OPTIONS**
  - **Access-Control-Allow-Headers**: ```content-type```

![fwd](/images/5.fwd/014.fwd.png) 

nhấn **Save** 
