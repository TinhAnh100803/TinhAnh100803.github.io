---
title : "Give Lambda permission to send emails"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 4.3 </b> "
---

Lambda needs access to SES:SendEmail.

1. Go to **Configuration** tab → select **Permissions**

![Lambda](/images/4.lambda/006.lambda.png)

2. Click on **role name** in the **Execution role** section
- In the **IAM Role** page → select **Add permissions** → **Attach policies**

![Lambda](/images/4.lambda/008.lambda.png)

3. Find and tick:
```AmazonSESFullAccess``` or create a separate **policy** that only grants the **ses:SendEmail** permission.

![Lambda](/images/4.lambda/007.lambda.png)

4. Click **Add permissions**