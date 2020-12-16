---
title: "Update your blueprint to use the Terraform module"
date: 2020-10-21T11:44:34+03:00
weight: 03
draft: false
---

1\. Remove mongodb artifact 
![03_page](/images/module4/04_page_1.png)
![03_page](/images/module4/04_page_2.png)

2\. Update input parameters
* Locate following block of code (inputs) in the blueprint:
![03_page](/images/module4/05_page_1.png)
* Append the following block of code to it:
```
- DB_USERNAME: adminuser
- DB_PASSWORD: 
    display_style: masked
    description: please set the master database password
    default_value: Welcome1234567+
```

3\. Locate the “promotion-manager-api” and “mongodb” sections of code in the blueprint. 
![03_page](/images/module4/06_page.png)

4\. Replace this section with the following code:
```
- promotions-manager-api:      
      depends_on: 
        - promotions-manager-docdb
      input_values:
        - API_PORT: $API_PORT
        - AWS_INSTANCE_TYPE: $AWS_INSTANCE_TYPE
        - DATABASE_HOST: $outputs.promotions-manager-docdb.connection_string
        - RELEASE_NUMBER: $RELEASE_NUMBER
        - API_BUILD_NUMBER: $API_BUILD_NUMBER
  
services:
  - promotions-manager-docdb:
      input_values:
        - USERNAME: $DB_USERNAME
        - PASSWORD: $DB_PASSWORD
        - SANDBOX_ID: ${SandboxID}

debugging:
  availability: on
```
Your new blueprint is now visible in Colony 
![03_page](/images/module4/09_page.png)

5\. Save and Commit your change to your Git repo
