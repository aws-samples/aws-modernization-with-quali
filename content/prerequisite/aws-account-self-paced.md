---
title: "Create an AWS account (Self-Paced)"
date: 2020-10-16T10:35:57+03:00
weight: 04
draft: false
---

__Note__: If you already have an AWS account with a role that has IAM Administrator permissions you can skip this step.

1\. [Create an AWS account](https://aws.amazon.com/getting-started/).

2\. Once you have created an AWS account, [create a IAM user](https://console.aws.amazon.com/iam/home?#/users$new) 

Enter a name and set a password.
![02_page](/images/prerequisite/create-aws-user.png)

Uncheck the __Require Password Reset__ box.
Click __Next: Set Permissions__.

Attach the __AdministratorAccess__ Permissions policy to the account. 
![02_page](/images/prerequisite/administrator-policy.png)

Click __Create User__.
![02_page](/images/prerequisite/create-user.png)