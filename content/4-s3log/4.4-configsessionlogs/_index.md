---
title : "Check operation"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4.4 </b> "
---

1. Go to the **Test** tab

![Lambda](/images/4.lambda/009.lambda.png)

2. Click Configure **test event**

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
    alert("✅ JSON copied!");
  });
}
</script>

3. Click **Test**