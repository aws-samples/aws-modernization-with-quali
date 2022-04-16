---
title: "Connect your AWS Cloud Account to Torque"
date: 2020-10-16T10:35:57+03:00
weight: 06
draft: false
---

To connect your AWS Cloud Account to Torque, follow the instructions below:

1\. Switch to the Admin Console using the drop-down on the left
 ![Admin Console](/images/prerequisite/admin_console_dropdown.png)

2\. Then, under the Cloud Accounts page, click the **Connect a Cloud** button
 ![Connect a Cloud](/images/prerequisite/admin_cloud_account.png) 

3\. Click the __AWS__ tile
 ![aws](/images/prerequisite/choose_cloud_account.png)

4\. Follow the instructions to create the Torque stack on your AWS account. Note the **Cloud Account Name** you provide to this cloud account, we'll use it later in this workshop. Use **aws-workshop** in the context of this workshop.
 ![authenticate](/images/prerequisite/authenticate_cloud_account.png)
 Click the **Launch Stack** button to open your AWS console with the CloudFormation stack details
 ![04_page](/images/prerequisite/11_page.png)
 Make sure you check the **I acknowledge that AWS CloudFormation might create IAM resources** checkbox, and click the Create Stack button
 ![04_page](/images/prerequisite/07_page.png)
 
5\. Wait until the stack creation completes. This should look something like this:
 ![04_page](/images/prerequisite/08_page.png)
 
6\. Click the __Outputs__ tab and copy the __RoleArn__ value
 ![04_page](/images/prerequisite/09_page.png)
 
7\. Return to Torque, paste the RoleArn value and click the **Authenticate** button to complete the process
 
 ![04_page](/images/prerequisite/paste_rolearn.png)
 
 ![04_page](/images/prerequisite/cloud_account_created.png)
 
