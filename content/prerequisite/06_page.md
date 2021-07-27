---
title: "Deploy a Sandbox from a sample blueprint"
date: 2020-10-16T10:35:57+03:00
weight: 08
draft: false
---

In this step, you will deploy a sandbox from the sample blueprint repository. This will enable you to test your setup and get familiar with the Torque UI. As a reminder, a __sandbox__ is a temporary environment that is automatically terminated once its time expires (ephemeral). 

1\. Open the **Sandbox Environments** page and click __New Sandbox__.
 ![06_page](/images/prerequisite/new_sandbox.png)
2\. Select a blueprint from the sample blueprint catalog and click **Next: Set Parameters**. The Dev & Test Environment deploys a simple JavaSpring website with a backend mySQL database.
 ![06_page](/images/prerequisite/select_sample_bp.png)
3\. Fill in the required parameters. In this case, only the **Sandbox Name** is required.
 ![06_page](/images/prerequisite/set_parameters.png)
Your new sandbox is being deployed on AWS. Note that this sample sandbox is deployed in the __eu-west-1__ region.
 ![06_page](/images/prerequisite/new_sandbox.png)
4\. Once your sandbox is deployed, you can browse the different tabs: **Summary**, **Applications**, **Infrastructure** to check that all the components have been deployed. You can also select the __Quick link__ from the **Summary** tab to directly access the JavaSpring website UI from the browser. You will explore more of the sandbox features in Module 2.
 ![06_page](/images/prerequisite/sandbox_deployed.png)
5\. When you're done, click on __End__ to manually terminate the sandbox, or let its time expire.
Note: You will __not__ use this sandbox for the rest of the workshop.
 ![06_page](/images/prerequisite/application_tab.png)
 

