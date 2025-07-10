---
title : "Phân quyền cho Lambda được phép gửi email"
date :  "`r Sys.Date()`" 
weight : 3
chapter : false
pre : " <b> 4.3 </b> "
---

 Lambda cần có quyền truy cập SES:SendEmail.

 1. Vào tab **Configuration** → chọn **Permissions**

![Lambda](/images/4.lambda/006.lambda.png)

2. Bấm vào **role name** ở phần **Execution role**
 - Trong trang **IAM Role** → chọn **Add permissions** → **Attach policies**


![Lambda](/images/4.lambda/008.lambda.png)

3. Tìm và tick chọn:

```AmazonSESFullAccess``` hoặc tạo **policy** riêng chỉ cấp quyền **ses:SendEmail**

![Lambda](/images/4.lambda/007.lambda.png)


4. Nhấn **Add permissions**