---
title: "Validate your deployment"
date: 2020-10-21T11:44:35+03:00
weight: 17
draft: false
---
In this step, you will check that the new service has been deployed in Torque and AWS. You will also discover how it is tied back to your Torque sandbox.
From the Torque sandbox, check that the service created from the Terraform module is listed.

1\. Navigate to the infrastructure tab.
![17_page](/images/module4/16_page.png)
2\. Login to the AWS console and navigate to the DocumentDB service. 
![17_page](/images/module4/17_page.png)
3\. Check the tags of the cluster that link back to the Torque context.
![17_page](/images/module4/18_page.png)
