---
title : "Enable CORS for Route"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 5.2 </b> "
---

1. Open the created **API Gateway**, select the API you just created **contact-form-api**, Go to the **Routes** menu

![fwd](/images/5.fwd/012.fwd.png)  

1. In the left column, select **CORS**

![fwd](/images/5.fwd/013.fwd.png)  


3. Configure **CORS**: 
  - **Access-Control-Allow-Origin**: *
  - **Access-Control-Allow-Methods**: select **POST**, **OPTIONS**
  - **Access-Control-Allow-Headers**: ```content-type```

![fwd](/images/5.fwd/014.fwd.png) 

Click **Save**