---
title : "Create API Gateway"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 5.1 </b> "
---


1. Access the **API Gateway Console**

![fwd](/images/5.fwd/001.fwd.png)  

2. Select **Create API**

![fwd](/images/5.fwd/002.fwd.png) 

3. Select **HTTP API** -> Click **Build**

![fwd](/images/5.fwd/003.fwd.png) 

4. Enter **API name** ```contact-form-api``` 
- **Integrations** click **Add integration** select **lambda** and select your **Lambda fuction**.

![fwd](/images/5.fwd/007.fwd.png) 


Click **Next**


5. Change Method from **ANY** → **POST**
Change **Resource path** from **/SendContactEmail** → **/send-email**

 ![fwd](/images/5.fwd/008.fwd.png)

 Click **Next**

6. **Define stages - optional** In this step, continue to click **Next**

![fwd](/images/5.fwd/009.fwd.png)

7. Check the information again and click **Create**

![fwd](/images/5.fwd/010.fwd.png)

8. After pressing **Create**, you will get the official **invoke URL**

![fwd](/images/5.fwd/011.fwd.png)

