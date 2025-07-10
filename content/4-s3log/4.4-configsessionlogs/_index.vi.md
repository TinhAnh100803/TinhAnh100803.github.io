---
title : "Kiểm tra hoạt động"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 4.4 </b> "
---

1. Vào tab **Test**


![Lambda](/images/4.lambda/009.lambda.png)

2. Nhấn Configure **test event**

Event name: testSend

Event JSON: 

<pre><code id="jsonData">
{
  "body": "{\"name\":\"Test User\",\"email\":\"test@example.com\",\"message\":\"Hello from the form!\"}"
}
</code></pre>

<script>
function copyJson() {
  const text = document.getElementById("jsonData").innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert("✅ Đã sao chép JSON!");
  });
}
</script>


3. Nhấn **Test**
