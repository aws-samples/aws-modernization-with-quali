---
title: "Deploy Jenkins Sandbox in Torque"
date: 2020-10-16T14:20:28+03:00
weight: 32
draft: false
---

1\. In Torque, navigate to the **Sandbox Environments** page, make sure you are in the **Ops-Tools** space,  and then click **New Sandbox"**
![32_page](/images/module3/32_page_2.png)

2\. Select the Jenkins blueprint and click **Next**
![32_page](/images/module3/33_page.png)

3\. Enter the required parameters:
* Sandbox Name: Jenkins_CI
* CS_TORQUE_TOKEN: Use the Jenkins token created in a previous steps
* SPACE_NAME: Trial
* AIM_ROLE: Set the value of the IAMRoleInstanceProfile key provided earlier by AWS
* BUCKET_NAME: Use the S3 bucket name you created
![32_page](/images/module3/34_page.png)

4\. Click **Launch Sandbox**
![32_page](/images/module3/35_page.png)

5\. Once the sandbox deployment is complete, click **Open Sandbox**

6\. In the **Sandbox Environments** > **Summary** page, wait until the application is fully deployed, then click its **Quick Link**

![32_page](/images/module3/36_page.png)

Congratulations! You've now automatically deployed an instance of Jenkins that can launch any blueprint configured in Torque! 
As the Ops team manager of Gourmet Inc, you may also use Torque to manage the new releases of the Jenkins platform as they become available.
