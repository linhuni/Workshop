---
title : "Create Public Subnet"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.1.2 </b> "
---

#### Create 2 Public Subnets

1. Click **Subnets**.
  + Click **Create subnet**.

![VPC](/images/2-Preparation/005-CreateVPC.png)

2. At the **Create subnet** page.
  + In the **VPC ID** section, click **Sample VPC**.
  + In the **Subnet name** field, enter **Public Subnet 1**.
  + In the **Availability Zone** section, select the first Availability zone.
  + In the field **IPv4 CIRD block** enter **10.0.0.0/24**.

![VPC](/images/2-Preparation/006-CreateVPC.png)
![VPC](/images/2-Preparation/007-CreateVPC.png)

3. Scroll to the bottom of the page, click **Create subnet**.
4. After successfully created Public Subnet, we will receive the notification
![VPC](/images/2-Preparation/008-CreateVPC.png)

5. Allow Automatic Allocation of Public IP Addresses for 2 Public Subnets
  + Slect **Subnets**
  + Select **Public Subnet 1**
  + Select **Actions**
  + Select **Edit subnet settings**
  + Select **Enable auto-assign public IPv4 address**
  + Select **Save**
![VPC](/images/2-Preparation/011-CreateVPC.png)
![VPC](/images/2-Preparation/012-CreateVPC.png)

The other subnet will be done the same

