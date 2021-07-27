---
title: "Check how the Jenkins pipeline script calls the Torque API"
date: 2020-10-16T14:20:29+03:00
weight: 40
draft: false
---
Let's check how Jenkins is configured to call the Torque API. The Jenkins Sandbox you deployed earlier preloaded the Torque plugin that provides pre-defined functions (Groovy code) that you can call when defining a new script. 

__Note__: If you have an existing Jenkins instance, you would install and configure the Jenkins plugin for Torque from the Torque __Integrations__ page and follow these [instructions](https://colonysupport.quali.com/hc/en-us/articles/360001035668).
 
1\. Click the "demo" link to the pre-loaded pipeline script.
 ![40_page](/images/module3/demo-jenkins.png)
2\. Click __Configure__.
 ![40_page](/images/module3/pipeline-configure.png)
3\. Navigate to the __Pipeline__ tab. Note that the "Use Groovy Sandbox" box is checked.
 ![40_page](/images/module3/pipeline-script-tab.png)
4\. Scroll down the script until you reach the "Integration Tests" stage. You use the __startSandbox()__ method to run sandbox from a blueprint passing all needed parameters.
 ![40_page](/images/module3/pipeline-script.png)
5\. Then, once the sandbox is ready, you use the __getEndpoint()__ function to take application endpoint, which could be used to perform some tests (not covered by this job).
 ![40_page](/images/module3/pipeline-script-endpoint.png)
6\. At the end you, terminate the sandbox with the __endSandbox()__ method, and move on to the next stage.
 ![40_page](/images/module3/pipeline-script-terminate.png)
 For more information, you can check out the [detailed syntax](https://colonysupport.quali.com/hc/en-us/articles/360001029427) of these functions in our documentation.
