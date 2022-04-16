---
title: "Create a promotion application blueprint for Developers"
date: 2020-10-22T15:07:26+03:00
draft: false
weight: 28
---
	
#### Your first task is to provide developers a self-service blueprint that has the entire promotion application deployed on a single VM (instead of the default three VMs), so they can do their unit testing and save infra cost.

Open the blueprint named promotions-manager-all-aws-dev from the Blueprints catalog.
Inside the blueprint view, you can see the 3 different components we need for this application:
![dev_env](/images/module1/dev_env.png)

In the __Infrastructure__ tab, you can verify in Torque that the current​ blueprint is configured to be deployed on three VM instances:

![39_page](/images/module1/39_page.png)
