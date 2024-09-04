---
title : "Create EC2 Instances"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3 </b> "
---

#### Create EC2 
1. Go to [EC2 console](https://console.aws.amazon.com/ec2).
  + Click on **Instances**.
  + Click **Launch instances**.
  + Enter the name of the EC2 **Public EC2**

![EC2](/images/3.CreateEC2/032-CreateEC2.png)

  + In the **Application and OS images**, we will leave default.

![EC2](/images/3.CreateEC2/033-CreateEC2.png)

  + In the **Keypair** section: 
    + Choose **Create new key pair**
    + Enter the name of the keypair - sample
    + Choose .pem mode
    + Cick **Create keypair**
![EC2](/images/3.CreateEC2/035-CreateEC2.png)
  + In the **Network settings**:
    + Choose the VPC is the **Sample VPC**
    + Select the **Public Subnet**
    + Select **Enable** Auto-assign Public IP
    + In the **Security Group** select **Existing security group** then choose the **Public subnet SG**
![EC2](/images/3.CreateEC2/036-CreateEC2.png)
    + Press **Launch instance**

**Notice:** After created EC2 we need to wait until the status of EC2 change from **Initializing** to **Running**, it means our EC2 is available 

2. Do the same with the **Private EC2**


