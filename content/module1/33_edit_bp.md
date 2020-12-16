---
title: "Edit the promotion-manager-dev blueprint​"
date: 2020-10-15T18:47:14+03:00
weight: 33
draft: false
---
In this step, you will edit a blueprint provided in your Git repository and modify it to meet the needs of your developers. Instead of 3 VMs, the promotion manager application components willa all be deployed on 1 VM.

1\. Edit __promotion-manager-dev.yaml__. You can find this file in the Git directory of your repo:
aws-workshop-colony/blueprints/

![43_page](/images/module1/edit_bp_git.png)
__Note__: this blueprint assumes you have permissions to deploy in “eu-west-1” region with your AWS account, if not update the value in the clouds section.

![43_page](/images/module1/pm_bp_view.png)

2\. For each application tier, uncomment #target: vm1​
![44_page](/images/module1/44_page.png)

3\. Commit your changes (Git)
![45_page](/images/module1/45_page.png)

Your blueprint will now automatically be synchronized to CloudShell Colony and available for deployment.