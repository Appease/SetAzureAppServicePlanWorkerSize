![](https://ci.appveyor.com/api/projects/status/0ehawprim572u9cx?svg=true)

####What is it?

An [Appease](http://appease.io) task template that sets an [Azure App Service plans](http://azure.microsoft.com/en-us/documentation/articles/azure-web-sites-web-hosting-plans-in-depth-overview/) worker size.

####How do I install it?

```PowerShell
Add-AppeaseTask `
    -DevOpName YOUR-DEVOP-NAME `
    -TemplateId SetAzureAppServicePlanWorkerSize
```

####What parameters are required?

#####Name
description: a `string` representing the name of the App Service plan.

#####ResourceGroupName
description: a `string` representing the name of the resource group of the App Service plan.

#####WorkerSize
description: a `string` representing the size of each worker VM allocated to the App Service plan  
known allowed values: `0`, `1`, `2`
