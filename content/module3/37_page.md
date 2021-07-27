---
title: "Deploy a Sandbox from Jenkins"
date: 2020-10-16T14:20:29+03:00
weight: 37
draft: false
---
Log in to the Jenkins server that you just deployed (use the default user "admin" and password "admin" if you did not change it in the sandbox parameter)
 ![37_page](/images/module3/37_page.png)
 
#### The default pipeline loaded with this Jenkins instance will automatically run the following steps:

1. Retrieve the latest code of the promotions-manager app from GitHub.
2. Build the artifact package (latest build).
3. Upload the artifact to the S3 repository.
4. Deploy the promotion application to AWS in a Torque Sandbox.
5. Run tests.
6. Terminate the promotion application.

