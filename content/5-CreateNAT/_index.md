---
title : "Create NAT gateway and test connection of private EC2"
date :  "`r Sys.Date()`" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---


#### Create NAT gateway

2. Go to [VPC console](https://console.aws.amazon.com/vpc)
   + Click **Elastic Ips** , then click **Allocate Elastic IP address**.

![EIP](/images/5.createNAT/044-createNAT.png)

   + Add the name of the EIP 
   + Click **Allocate**

![EIP](/images/5.createNAT/045-createNAT.png)
![EIP](/images/5.createNAT/046-createNAT.png)

2. Create **NAT gateway**.
   + Click on **Create NAT gateway**.

![NAT](/images/5.createNAT/047-createNAT.png)
![NAT](/images/5.createNAT/048-createNAT.png)

3. Test conenction of private EC2 with connection
   + Enter **ping amazon.com -c5**
![TEST](/images/5.createNAT/051-testconnection.png)