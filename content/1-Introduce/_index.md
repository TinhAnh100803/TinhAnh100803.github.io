---
title : "Introduction"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**Static website with contact form processing** is a popular model in building simple, lightweight, easy-to-deploy websites such as company introduction pages, personal portfolios or landing pages to collect customer feedback.

In this workshop, you will be guided on how to deploy a static website using **Amazon S3** for storage, **CloudFront** for global content delivery and secure connection via HTTPS. In particular, the **contact form** will not need a traditional backend but instead use **Serverless** architecture including:

- **Amazon API Gateway**: routes requests from forms
- **AWS Lambda**: processes form content
- **Amazon SES**: sends email notifications about contact content

**You will learn how to:**

- Build a static and public website on S3
- Deliver content via CDN (CloudFront) with HTTPS
- Create a serverless API to handle form submissions from clients
- Send automated emails via SES
- Leverage serverless cloud infrastructure