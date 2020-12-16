---
title: "Deploy a Sandbox from a sample blueprint"
date: 2020-10-16T10:35:57+03:00
weight: 08
draft: false
---

In this step, you will deploy a sandbox from the sample blueprint repository. This will enable to test your setup and get familiar with the Colony UI. As a reminder, a __sandbox__ is a temporary environment that is automatically terminated once its time expires (ephemeral). 

1\. Browse the Sandbox environment tab and click on __New Sandbox__.
 ![06_page](/images/prerequisite/new_sandbox.png)
2\. Select a blueprint from the sample blueprint catalog. The Dev & Test Environment will deploy a simple JavaSpring website with a backend mySQL database.
 ![06_page](/images/prerequisite/select_sample_bp.png)
3\. Provide the required parameters. In this case, only the Sandbox name is required.
 ![06_page](/images/prerequisite/set_parameters.png)
Your new sandbox will now be automatically be deployed on AWS infrastructure. Note that this sample sandbox is deployed in __eu-west-1__ region.
 ![06_page](/images/prerequisite/new_sandbox.png)
4\. Once your sandbox is deployed, you can browse the different tabs: "summary", "application", "infrastructure" to check that all the components have been deployed. you can also click on the __Quick link__ from the Summary tab that will lead you directly to the JavaSpring website UI. You will explore more of the sandbox features in Module 2.
 ![06_page](/images/prerequisite/sandbox_deployed.png)
 5.\ Once done, you can click on __End__ to manually terminate the sandbox, or let its time expire.
 Note: you will __not__ use this sandbox for the remaining of the workshop.
 ![06_page](/images/prerequisite/application_tab.png)
 
 
