---
title : "Create Security Group"
date : "`r Sys.Date()`"
weight : 6
chapter : false
pre : " <b> 2.1.6 </b> "
---

#### Create Security Group

1. Go to [VPC service management console](https://console.aws.amazon.com/vpc)
  + Click **Security Group**.

![SG](/images/2.preparation/025-CreateSecurity.png)

2. At the create security group page
    + Enter the name of the security group - **Public subnet SG**
    + Add description - **Allow SSH and ping for servers in public subnets**
    + Select the **Sample VPC**
    + In the **Inbound rule** we will set up as the picture below.
![SG](/images/2.preparation/026-CreateSecurity.png)
![SG](/images/2.preparation/027-CreateSecurity.png)
    + With the **Private subnet SG** we will do as the same but in the **Inbound rule** we will set as below
![SG](/images/2.preparation/028-CreateSecurity.png)

3. After successfully created the security group. We will have two groups as below
![SG](/images/2.preparation/029-CreateSecurity.png)

