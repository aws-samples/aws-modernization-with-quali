---
title: "Cleanup"
chapter: false
weight: 0
---

- **Your Torque trial instance** - The Torque trial instance that you used in this workshop will automatically be terminated after 30 days. There isn't anything you need to do. If you would like keep it, you can upgrade to a paying plan. [Contact us](https://info.quali.com/contact-us) for more details.

- **Amazon Resources** - To cleanup your Amazon S3 resources, go to your [S3 service console](https://s3.console.aws.amazon.com/s3/home#/listBuckets). Select the artifact-repo-promotionapp bucket and click **Empty**.
![Empty S3 bucket](/images/cleanup/delete-s3-3.png)
 Click **Delete** to completely remove the S3 bucket from your account.
![Delete S3 bucket](/images/cleanup/delete-s3-4.png)
 This completes the cleanup activities.
 
 __Note__: Torque takes care of all the sandbox resource cleanup out of the box, so you don't have to worry about left-over resources.
 
