---
title: "Create a promotion application blueprint for load testing​"
date: 2020-10-15T18:47:14+03:00
weight: 36
draft: false
---

* Your next task will be to provide application environments for the load testing QA certification. 
* In this case, you will increase the number of VMs for the application UI tier from 1 to 3. The ELB load balancer will be automatically configured

![46_page](/images/module1/46_page.png)

Edit promotions-manager-all-aws-loadtest.yaml (in the /blueprint directory in your Git repo) and uncomment the "#instances: 3 for the UI tier​" line

![46_page](/images/module1/48_page.png)
 
 Commit your changes
 
 ![46_page](/images/module1/49_page.png)

