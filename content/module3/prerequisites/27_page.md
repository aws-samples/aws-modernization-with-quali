---
title: "Create an S3 role using a Cloud Formation template"
date: 2020-10-16T14:20:28+03:00
weight: 27
draft: false
---

In the next steps, you will create an S3 role that will give Jenkins permission to upload the Promotion Manager application build to the artifact repository you created in module 1. The role value will be used as an input to the Jenkins Sandbox deployment. Once Jenkins is deployed, it will use this role as a parameter of the pipeline jobs that you will run (see [Deploy a Sandbox from Jenkins](https://quali.awsworkshop.io/module3/37_page.html).

1\. Open AWS in a browser and navigate to the [__CloudFormation__](https://console.aws.amazon.com/cloudformation/) service

2\. Click __Create stack__

![27_page](/images/module3/27_page.png)

3\. In the drop-down list that appears, select __With new resources (standard)__

4\. Under __Template source__, select __Upload a template file__

5\. Click __Choose file__

6\. Upload __s3_bucket_access.template__ from the __/jenkins__ directory of the workshop's repo you created in Module 1.
You may select the file from your local clone of the workshop's Git repo, or use the URL of that file in the original repo:
https://github.com/QualiSystemsLab/aws-workshop-torque/blob/master/jenkins/s3_bucket_access.template

![27_page](/images/module3/28_page.png)

7\. Click __Next__

8\. Enter a name for the stack (e.g. "S3role") and specify the S3 bucket name as the S3 bucket name in __Parameter__

![27_page](/images/module3/29_page.png)

9\. Click __Next__

10\. In the __Configure stack options__ page, click __Next__ again

11\. In the __Review__ page, scroll to the bottom and check the acknowledgement checkbox

![27_page](/images/module3/30_page.png)

12\. Click _Create stack__

13\. Wait for the new role to be created - you might want to click the refresh button on the top-right of the __Events__ table

14\. Once the role is created, open the __Outputs__ tab

15\. Save the value of the `IAMRoleInstanceProfile` key. It will serve as an input for your Jenkins sandbox

![27_page](/images/module3/31_page.png)
