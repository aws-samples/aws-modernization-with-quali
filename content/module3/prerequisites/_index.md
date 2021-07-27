---
title: "Prerequisites"
date: 2020-10-29T09:44:46+02:00
weight: 1
---
### As a member of the Ops platform tools team at Gourmet Inc, you will automatically deploy and configure Jenkins using Torque.

---
**NOTE:** This step would typically be performed ahead of time. Torque can be used to deploy platform tools and keep them up-to-date with the latest version.\\

---

Your goal in the next few steps is to deploy a new Jenkins instance in AWS EC2 using Torque. This instance will be pre-configured with a sample pipeline job that can be used to automatically deploy the promotion manager application.

Complete information about this setup is available in the [Readme](https://github.com/QualiSystemsLab/jenkins-torque/blob/master/README.md) file of the Github repository. 

In order to deploy Jenkins from Torque, you will first create a new "Space" that will model the Ops platform team workspace. You will then generate a couple of input parameters required for Jenkins to work in the context of your promotion manager application and Torque: a IAM role to upload your artifacts to the S3 repo, and a token that allows Jenkins to run the Torque REST API.
