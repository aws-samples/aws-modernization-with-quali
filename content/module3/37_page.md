---
title: "Deploy a Sandbox from Jenkins"
date: 2020-10-16T14:20:29+03:00
weight: 37
draft: false
---
Login to the Jenkins server that you just deployed (use the default "admin" password if you did not change it in the sandbox parameter)
 ![37_page](/images/module3/37_page.png)
 
#### The default pipeline loaded with this Jenkins instance will automatically run the following steps:

1. Retrieve latest code of the promotion app from Git
2. Build artifact package (latest build)
3. Upload Build to S3 repository
4. Deploy the promotion application to AWS in a Colony Sandbox
5. Run tests
6. Terminate the promotion application

