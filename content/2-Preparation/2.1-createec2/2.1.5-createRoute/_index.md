---
title : "Create Route Table"
date : "`r Sys.Date()`"
weight : 5
chapter : false
pre : " <b> 2.1.5 </b> "
---
#### Create route table

Go to [VPC service management console](https://console.aws.amazon.com/vpc)
+ Click **Route tables**.
+ Click **Create route table**.

![ROUTE](/images/2-Preparation/018-Createroute.png)

+ Enter name of the route**Public table**.
+ Choose the VPC as **Sample VPC**.
+ Click **Create route table**.

![ROUTE](/images/2-Preparation/019-Createroute.png)


After created route table for the subnets. We will edit the route of the public table
+ Click **Edit route**.

Because we want it to be connected with the Internet so we will choose the Destination and Route as 0.0.0.0/0 and our internet gateway.

![ROUTE](/images/2-Preparation/021-Createroute.png)

+ Click **Save changes**

Then we will associate our route table to our subnets.

+ Click **Subnet association**
+ Click **Edit Subnet association**

![ROUTE](/images/2-Preparation/022-Createroute.png)

+ Select **Public subnets**

![ROUTE](/images/2-Preparation/023-Createroute.png)

+ Click **Save changes**
![ROUTE](/images/2-Preparation/024-Createroute.png)

+ With **Private route** we only need to edit the **inbound rule** and the **subnet associations**.
![ROUTE](/images/2-Preparation/049-createroute.png)
![ROUTE](/images/2-Preparation/050-createroute.png)



    