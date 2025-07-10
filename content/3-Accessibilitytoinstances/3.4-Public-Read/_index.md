---
title : "Grant public access"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 3.4. </b> "
---

1. Assign **Bucket Policy**
- Go to the **Permissions** tab and scroll down to **Bucket policy**

![Connect](/images/3.connect/012-connect.png)

2. Paste the following code, remembering to replace **YOUR_BUCKET_NAME**:

<pre><code id="bucketPolicy">
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicRead",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::YOUR_BUCKET_NAME/*"
    }
  ]
}
</code></pre>

<script>
function copyToClipboard() {
  const text = document.getElementById("bucketPolicy").innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert("Đã sao chép!");
  });
}
</script>

After pasting, click **Save changes**.

![Connect](/images/3.connect/013-connect.png)