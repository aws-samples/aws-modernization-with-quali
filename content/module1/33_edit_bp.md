---
title: "Edit the promotion-manager-all-aws-dev blueprint​"
date: 2020-10-15T18:47:14+03:00
weight: 33
draft: false
---
In this step, you will edit a blueprint provided in your Git repository and modify it to meet the needs of your developers. Instead of three VMs, the promotion manager application components will all be deployed on one VM.

1\. Edit __promotion-manager-all-aws-dev.yaml__. You can find this file in the Git directory of your repo:
aws-workshop-torque/blueprints/

![43_page](/images/module1/edit_bp_git.png)
---
**NOTE**: This blueprint assumes you have permissions to deploy your VMs in the "eu-west-1" region with your AWS account; if not, update the value in the __clouds__ section accordingly.
Also, it will use the "aws-workshop" cloud account we created in the previous steps. If you called it differently, you'll need to update this name as well.

---

![43_page](/images/module1/pm_bp_view.png)

2\. For each application tier, uncomment "#target: vm1​":
![44_page](/images/module1/44_page.png)

3\. Commit your changes and push to your repository

Torque will get the latest updates automatically whenever you update your blueprint repository.
