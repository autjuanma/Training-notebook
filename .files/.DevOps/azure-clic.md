
[AZURE CLI]
# Create resource
[az ad sp create-for-rbac --name http://PU1app]

[
  {
    "cloudName": "AzureCloud",
    "homeTenantId": "698f79a6-5234-4fb0-9610-4413bf71bf5a",
    "id": "232a7501-eeae-43d1-b6ca-37cc07cc5a6f",
    "isDefault": true,
    "managedByTenants": [],
    "name": "Azure subscription 1",
    "state": "Enabled",
    "tenantId": "698f79a6-5234-4fb0-9610-4413bf71bf5a",
    "user": {
      "name": "juantousmcro@outlook.com",
      "type": "user"
    }
  }
]


az ad sp create-for-rbac --name http://PU1app

{
  "appId": "acf3b2e5-3dd9-44c2-8444-7552a523c0a1",
  "displayName": "PU1app",
  "name": "http://PU1app",
  "password": "lz~X87fMfD3ZZIom1X5ZckeMsgOzmdf98y",
  "tenant": "698f79a6-5234-4fb0-9610-4413bf71bf5a"
}

 az role assignment list --assignee  <app id from earlier > i.e. something like 5c0e5186-737c-42ad-881e-16d735ac3dab
 az role assignment list --assignee  <app id from earlier > 

# Asegurarse que el rol no se que <Contributor>

[
  {
    "canDelegate": null,
    "condition": null,
    "conditionVersion": null,
    "description": null,
    "id": "/subscriptions/232a7501-eeae-43d1-b6ca-37cc07cc5a6f/providers/Microsoft.Authorization/roleAssignments/11a9741b-f2e3-4d1b-bcb2-87e543f64cd8",
    "name": "11a9741b-f2e3-4d1b-bcb2-87e543f64cd8",
    "principalId": "20875bf0-1ed3-41de-bb32-f1b5b9176622",
    "principalName": "http://PU1app",
    "principalType": "ServicePrincipal",
    "roleDefinitionId": "/subscriptions/232a7501-eeae-43d1-b6ca-37cc07cc5a6f/providers/Microsoft.Authorization/roleDefinitions/b24988ac-6180-42a0-ab88-20f7382dd24c",
    "roleDefinitionName": "Contributor",
    "scope": "/subscriptions/232a7501-eeae-43d1-b6ca-37cc07cc5a6f",
    "type": "Microsoft.Authorization/roleAssignments"
  }
]

# login Cli
az login --use-device-code
ET36RERXW
ET36RERXW


az login --service-principal -u <APP_ID> --password <PWD> --tenant <TENANT_ID>
az login --service-principal -u acf3b2e5-3dd9-44c2-8444-7552a523c0a1 --password lz~X87fMfD3ZZIom1X5ZckeMsgOzmdf98y --tenant 698f79a6-5234-4fb0-9610-4413bf71bf5a


### --->
Client Id for connecting to the endpoint. Refer to Azure Service Principal link on how to create Azure Service Principal.
[
  {
    "cloudName": "AzureCloud",
    "homeTenantId": "698f79a6-5234-4fb0-9610-4413bf71bf5a",
    "id": "232a7501-eeae-43d1-b6ca-37cc07cc5a6f",
    "isDefault": true,
    "managedByTenants": [],
    "name": "Azure subscription 1",
    "state": "Enabled",
    "tenantId": "698f79a6-5234-4fb0-9610-4413bf71bf5a",
    "user": {
      "name": "acf3b2e5-3dd9-44c2-8444-7552a523c0a1",
      "type": "servicePrincipal"
    }
  }
]

>>>>>>>>>>>>>>>>>>>>>>>>>

Tenant ID
Password = Service Principal Key
User name (also referred to as App ID or Service Principal Client ID)

>>>>>>>>>>>>>>>>>>>>>>>>>Client Id for connecting to the endpoint. Refer to Azure Service Principal link on how to create Azure Service Principal.



# Officcial step



1. MyResourceGroup=arm-vscode
2  MyStorageAccount=arroyodevopsroberto



# Test


# Example 1: Test deployment with a custom template object and parameter file

Test-AzResourceGroupDeployment -ResourceGroupName "ContosoEngineering" -TemplateObject $TemplateObject -TemplateParameterFile "D:\Azure\Templates\EngSiteParams.json"



# Example 2: Test deployment via template file and parameter file
PS C:\> Test-AzResourceGroupDeployment -ResourceGroupName testRG01 -TemplateFile "D:\Azure\Templates\sampleDeploymentTemplate.json" -TemplateParameterFile "D:\Azure\Templates\sampleDeploymentTemplateParams.json"


PS C:\> Test-AzResourceGroupDeployment -ResourceGroupName testRG01 -TemplateFile "" -TemplateParameterFile "D:\Azure\Templates\sampleDeploymentTemplateParams.json"









