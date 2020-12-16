---
title: "Create an S3 role using a Cloud Formation template"
date: 2020-10-16T14:20:28+03:00
weight: 27
draft: false
---
In the next few steps, you will create an S3 role that will give Jenkins permission to upload the promotion manager application build to the artifact repository you created in module 1. The role value will be used as an input to the Jenkins Sandbox deployment. Once Jenkins is deployed, it will use this role as a parameter of the pipeline jobs that you will run (see __Deploy a Sandbox from Jenkins__ step in module 3).

1\. Navigate to "Services: Cloud Formation" to Create Stack
![27_page](/images/module3/27_page.png)
2\. Upload template file s3_bucket_access.template provided in the workshop Git repo (__jenkins__ directory)
![27_page](/images/module3/28_page.png)
3\. Enter a name for the stack and specify the S3 bucket name as input parameter 
![27_page](/images/module3/29_page.png)
4\. Follow the __Next__ screens until you get to the stack creation button (check box at the bottom)
![27_page](/images/module3/30_page.png)
5\. S3 role is now created. Save the value. This role will be an input of your Jenkins sandbox 
![27_page](/images/module3/31_page.png)