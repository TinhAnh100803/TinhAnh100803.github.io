---
title : "Create a new Bucket on Amazon S3"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---
**Overview**: 
Amazon Simple Storage Service (Amazon S3) is an on-demand, scalable object storage service that delivers the highest levels of data availability, security, and performance. 

S3 is built to meet the needs of customers of all sizes and industries, and can be used to store and protect any amount of data.

S3 can be used for a wide range of use cases, including data warehouses, websites, mobile applications, backup and restore, archiving, enterprise applications, IoT devices, and big data analytics. Additionally, Amazon S3 provides easy-to-use management features that allow you to organize your data and configure access controls to meet your specific business, organizational, and compliance needs. 

Amazon S3 is designed to provide 99.9999999999% (11 9’s) durability and stores data for millions of applications for companies around the world.

![SSMPublicinstance](/images/S3.png)

1. First, we will create an S3 bucket:

- Go to AWS Management Console.
- Search for S3.
- Select S3.

![Connect](/images/3.connect/001-connect.png)

2. In the **S3** interface, select **Create bucket**.

 ![Connect](/images/3.connect/002-connect.png)

3. In the Create bucket interface:

- Bucket name: enter ```aws-first-cloud-journey```.

- AWS Region: select the region you want.

- For Object Ownership, select ACLs disabled (recommended).

![Connect](/images/3.connect/003-connect.png)
**Note**: Since **Bucket name** is globally unique, using the same name as above will result in a message **“Bucket with the same name already exists”**. Therefore, you need to add a few numbers after it to make your **Bucket name** fit the policy.

![Connect](/images/3.connect/004-connect.png)

4. Uncheck **"Block all public access"** in the **Object Ownership & Permissions** section

![Connect](/images/3.connect/005-connect.png)

5. Click **Create bucket** to initialize.

![Connect](/images/3.connect/006-connect.png) 