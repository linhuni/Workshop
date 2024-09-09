---
title : "Create Private Subnet"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 2.1.3 </b> "
---

#### Create 2 Private Subnets

1. Click **Subnets**.
   + Click **Create subnet**.

![VPC](/images/-Preparation/0090-CreateVPC.png)



2. At the **Create subnet** page.
   + In the **VPC ID** section, click **Sample VPC**.
   + In the **Subnet name** field, enter **Private Subnet 1**.
   + In the **Availability Zone** section, select the first Availability zone.
   + In the field **IPv4 CIRD block** enter **10.0.0.1/24**.

![VPC](/images/2-Preparation/010-CreateVPC.png)
![VPC](/images/2-Preparation/009-CreateVPC.png)

3. Scroll to the bottom of the page, click **Create subnet**.

The next step is to create the necessary security groups for the lab.