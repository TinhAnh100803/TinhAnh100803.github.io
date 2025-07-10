---
title : "Cấp quyền truy cập công khai"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 3.4. </b> "
---

1. Gán **Bucket Policy**
- Vào tab **Permissions** kéo xuống **Bucket policy**

![Connect](/images/3.connect/012-connect.png)

2. Dán đoạn mã sau, nhớ thay **YOUR_BUCKET_NAME**:
   
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

Sau khi dán xong, nhấn **Save changes**.

![Connect](/images/3.connect/013-connect.png)