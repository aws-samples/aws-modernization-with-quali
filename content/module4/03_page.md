---
title: "Update your blueprint to use the Terraform module"
date: 2020-10-21T11:44:34+03:00
weight: 03
draft: false
---

1\. Remove the mongodb artifact. 
![03_page](/images/module4/04_page_1.png)
![03_page](/images/module4/04_page_2.png)

2\. Locate the inputs section:
![03_page](/images/module4/05_page_1.png)

3\. Add the following to the section:
```
- DB_USERNAME: adminuser
- DB_PASSWORD: 
    display_style: masked
    description: please set the master database password
    default_value: Welcome1234567+
```

3\. Locate the “promotion-manager-api” and “mongodb” sections. 
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

5\. Save your changes, commit to your local repo and push to Github.

Your new blueprint is now visible in Torque.
![03_page](/images/module4/09_page.png)
