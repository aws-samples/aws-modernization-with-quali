---
title: "Add blueprint repository to the Ops-Tools space"
date: 2020-10-16T14:20:26+03:00
weight: 10
draft: false
---

For this module, we will use an existing public repository in our Ops-Tools space.
Open the Repositories tab in the space settings, and add the following public repository: https://github.com/QualiSystemsLab/jenkins-torque
 ![10_page](/images/module3/10_page.png)
 
The Jenkins repository is now listed
 ![10_page](/images/module3/12_page_1.png)

Next, let's add an Artifact Repository:

1\. Click the __Add a Repository__ button in the Artifact Repository section

2\. Select __AWS S3__.
![13_page](/images/module3/14_page.png)

3\. From the drop-down lists, select the cloud provider (aws-workshop) and the S3 bucket you previously created in Module 1.
![13_page](/images/module3/ops_repos.png)
