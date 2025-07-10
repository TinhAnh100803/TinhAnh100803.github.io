---
title : "Cài đặt mã xử lý gửi email"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 4.2 </b> "
---


1. Sau khi tạo xong **function**, bạn sẽ được đưa vào trang chi tiết.

![Lambda](/images/4.lambda/004.lambda.png)


2. Cuộn xuống phần code **Source**


![Lambda](/images/4.lambda/005.lambda.png)
 

3. Thay thế toàn bộ nội dung mặc định bằng đoạn code sau:

<pre><code id="emailCode">
import json
import boto3
import os

ses = boto3.client('ses', region_name='ap-southeast-1')

def lambda_handler(event, context):
    # Xử lý preflight CORS (OPTIONS request)
    if event['requestContext']['http']['method'] == 'OPTIONS':
        return {
            'statusCode': 200,
            'headers': {
                'Access-Control-Allow-Origin': '*',
                'Access-Control-Allow-Headers': 'Content-Type',
                'Access-Control-Allow-Methods': 'OPTIONS,POST'
            },
            'body': json.dumps('Preflight OK')
        }

    body = json.loads(event['body'])

    name = body.get('name')
    email = body.get('email')
    message = body.get('message')

    subject = f"Liên hệ mới từ {name}"
    body_text = f"Email: {email}\n\nNội dung:\n{message}"

    # Gửi email qua SES
    response = ses.send_email(
        Source=os.environ['SENDER_EMAIL'],
        Destination={'ToAddresses': [os.environ['RECEIVER_EMAIL']]},
        Message={
            'Subject': {'Data': subject},
            'Body': {
                'Text': {'Data': body_text}
            }
        }
    )

    return {
        'statusCode': 200,
        'headers': {
            'Access-Control-Allow-Origin': '*',
            'Access-Control-Allow-Headers': 'Content-Type',
            'Access-Control-Allow-Methods': 'OPTIONS,POST'
        },
        'body': json.dumps({'message': 'Gửi email thành công!'})
    }

</code></pre>

<script>
function copyCode() {
  const text = document.getElementById("emailCode").innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert("✅ Đã sao chép đoạn mã!");
  });
}
</script>

<div style="border-left: 4px solid #f39c12; padding: 10px; background-color: #fff8e1;">
  <strong>⚠️ Lưu ý:</strong>
  <ul>
    <li>SENDER_EMAIL:<code> bằng email bạn muốn nhận thư.</code> </li>
    <li>RECEIVER_EMAIL:<code>Email mà bạn muốn nhận tin nhắn liên hệ (người nhận)</code></li>
  </ul>
</div>
