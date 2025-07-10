---
title : "Tạo API Gateway"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 5.1 </b> "
---


1. Truy cập **API Gateway Console**

![fwd](/images/5.fwd/001.fwd.png)  

2. Chọn **Create API**

![fwd](/images/5.fwd/002.fwd.png) 

3. Chọn **HTTP API** -> Bấm **Build**

![fwd](/images/5.fwd/003.fwd.png) 

4. Nhập tên **API name** ```contact-form-api``` 
- **Integrations** nhấn chọn **Add integration** chọn **lambda** và chọn **Lambda fuction** của bạn.

![fwd](/images/5.fwd/007.fwd.png) 


 Nhấn **Next**


5. Đổi Method từ **ANY** → **POST**
   Đổi **Resource path** từ **/SendContactEmail** → **/send-email**

 ![fwd](/images/5.fwd/008.fwd.png)

 Nhấn **Next**

6. **Define stages - optional** Ở bước này tiếp tục nhấn **Next**

![fwd](/images/5.fwd/009.fwd.png)

7. Kiểm tra lại thông tin và nhấn **Create** 

![fwd](/images/5.fwd/010.fwd.png)

8. Sau khi nhấn **Create**, bạn sẽ nhận được **URL invoke** chính thức

![fwd](/images/5.fwd/011.fwd.png)