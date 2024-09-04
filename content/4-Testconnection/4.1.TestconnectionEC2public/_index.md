---
title : "Test connection"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 4.1. </b> "
---

#### Test connection
1. Test connection of EC2 with SSH

    1.  Go to the [EC2 console](https://console.aws.amazon.com/ec2):
        + Choose the **Instances**.
        + Select the **Public EC2**.
        + In **Detail** part, copy the **Public IPv4 address** of the instance.

    ![Test](/images/4.testconnection/037-testconnection.png)

    2. Open Terminal ( On Mac OS) :
        + Use cd command to go to the Folder containing the .pem key.
        + Here, enter the command **chmod 400 sample.pem** to allow to read the file.
        + Enter the command **ssh -i sample.pem ec2-user@Public IPv4 address**  to connect ssh to the ec2 public.
        + Enter the command **ping amazon.com -c5** to check if the instance is connected to ssh or not.

    ![Test](/images/4.testconnection/038-testconnection.png)
    ![Test](/images/4.testconnection/039-testconnection.png)

2. Test connect between priavte and public EC2
    
    1. Staying in the ec2-user above:
        + Enter the command **ping Private IPv4 address -c5** 
        ![Test](/images/4.testconnection/040-testconnection.png)

3. Test connection of private EC2 and SSH

    1. Because we can't connect directly Internet to private EC2, we have to connect the Internet to private EC2 through public EC2 and NAT gateway. 
        + Open Terminal ( On Mac OS)
        + Use cd command to go to the Folder containing the .pem key.
        + Here, enter the command **scp -i sample.pem sample.pem ec2-user@47.129.154.215:~/.ssh** to copy the .pem file from the local host to the remote instance
        + Connect to the EC2 public 
        + Use cd command to go to the file **.ssh** then use **ls** to check if the .pem file here or yet
        + Here, enter the command **chmod 400 sample.pem** to allow to read the file.
        + Enter the command **ssh -i sample.pem ec2-user@PPrivate IPv4 address**  to connect ssh to the private ec2.
        + Use the command **ping amazon.com -c5** to check if the private EC2 connect to Internet or not. 
        We can see that the private EC2 can't connect to the Internet without the NAT gateway. So we need to create a

    ![Test](/images/4.testconnection/041-testconnection.png)
    ![Test](/images/4.testconnection/042-testconnection.png)
  




    


