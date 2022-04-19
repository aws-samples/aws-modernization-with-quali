---
title: "Check how the Jenkins pipeline script utilizes Torque"
date: 2020-10-16T14:20:29+03:00
weight: 40
draft: false
---
Let's check how Jenkins is configured to work with Torque. The Jenkins Sandbox you deployed earlier preloaded the Torque plugin that provides pre-defined methods (Groovy code) that you can call when defining a new script. 

__Note__: If you have an existing Jenkins instance, you would need to install and configure the Jenkins plugin for Torque. Follow these [instructions](https://community.qtorque.io/jenkins-67/installing-the-jenkins-plugin-311) to learn more.
 
1\. Click the "demo" link to the pre-loaded pipeline script.
 ![40_page](/images/module3/demo-jenkins.png)
2\. Click __Configure__.
 ![40_page](/images/module3/pipeline-configure.png)
3\. Switch to the __Pipeline__ tab (or scroll down to get to the pipeline script). Note that the "Use Groovy Sandbox" box is checked.
 ![40_page](/images/module3/pipeline-script-tab.png)
4\. Scroll down the script until you reach the "Integration Tests" stage. We use the __startSandbox()__ method to start a sandbox from a blueprint, passing all the needed parameters.
 ![40_page](/images/module3/pipeline-script.png)
5\. Then, once the sandbox is ready, we use the __getEndpoint()__ function (which is defined further on in this script) to get new application endpoint url from the sandbox, which could be used later to perform some tests (not covered by this job).
 ![40_page](/images/module3/pipeline-script-endpoint.png)
6\. At the end, we stop the sandbox with the __endSandbox()__ method, and move on to the next stage.
 ![40_page](/images/module3/pipeline-script-terminate.png)
 For more information, you can check out the [detailed syntax](https://community.qtorque.io/jenkins-67/launching-a-sandbox-from-jenkins-pipeline-277) of these methods in our documentation.
