# YAML template to deploy Azure Function App with PowerShell Core Infrastructure (Resources)
This repo deploys Azure FunctionApp, Application Insights, Storage Account, and AppService infrastructure (resources). You can combine this repo with deploying your own function if you know how, read the steps below before running your own CI pipeline.

DO THIS BEFORE RUNNING THE CI PIPELINE:

1. Create Azure KeyVault
2. Create Service Connection in Azure DevOps. Go to project settings -> service connection -> select ur service connection or make one if you dont have 1 -> edit -> copy the WHOLE subscription ID 
3. Go to KeyVault -> Access Policies -> + Add Access Policy -> (optional) select all for Key, Secret, and Certificate permissions -> Select principal -> paste the WHOLE subscription ID in the select a principal search box -> you should find the service connection you created in step 2 then click add
4. Push this repo into ur Azure DevOps repo
5. Change lines 3,4,5,27,61 to your own settings (IMPORTANT)
