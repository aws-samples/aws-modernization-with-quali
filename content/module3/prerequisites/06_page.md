---
title: "Create and Configure a new “Ops-Tools” space in Torque"
date: 2020-10-16T14:20:26+03:00
weight: 2
draft: false
---
In the next few steps, you will create and configure a new "space" in Torque. A space is a way to provide a specific team with access to the resources they need. It is part of the proper governance practices a company like Gourmet Inc wants to enforce. In our scenario, we are creating a space for the Platform Ops team to deploy and manage tools like Jenkins.

1\. Go to the __Admin Console__ area.
 ![06_page](/images/module3/admin_console_link.png)

2\. Click __Spaces__ on the left and create a new __Ops-Tools__ space. You can also choose a space color and icon to make it unique.
 ![06_page](/images/module3/06_page.png)

You will use this space to manage Ops platforms such as Jenkins. 
 ![06_page](/images/module3/07_page.png)

3\. To add your AWS cloud account to the __Ops-Tools__ space, click __Cloud Accounts__ on the left.

4\. Manage the existing __aws-workshop__ cloud account. 
![06_page](/images/module3/09_page.png)

5\. Add a new space to the existing ones. Select the __Ops-Tools__ space from the dropdown and click the __Configure__ button.
![09_page1](/images/module3/09_page_1.png)
The Ops-Tools should now be one of the spaces that can use this cloud account. It should look like this:
![09_page2](/images/module3/09_page_2.png)
6\. To verify, you can go to the Ops-Tools space the dropdown in the top left of the page, then click __Settings__ and then view the __Cloud Accounts__ tab. Our aws-workshop should now appear there. 
![09_page3](/images/module3/09_page_3.png)
