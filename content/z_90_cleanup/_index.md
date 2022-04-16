---
title: "Cleanup"
chapter: true
draft: false
weight: 90
--- 

- **Your Torque instance** - The Torque free instance that you used in this workshop will remain active for as long as you need it. If you need more out of if, you can upgrade to a paying plan. [Contact us](https://info.quali.com/contact-us) for more details.

- **Amazon Resources** - To cleanup your Amazon S3 resources, go to your [S3 service console](https://s3.console.aws.amazon.com/s3/home#/listBuckets). Select the artifact-repo-promotionapp bucket and click **Empty**.
![Empty S3 bucket](/images/cleanup/delete-s3-3.png)
 Click **Delete** to completely remove the S3 bucket from your account.
![Delete S3 bucket](/images/cleanup/delete-s3-4.png)
 This completes the cleanup activities.
 
 __Note__: Torque takes care of all the sandbox resource cleanup out of the box, so you don't have to worry about left-over resources.
