# az cli API

[
  {
    "cloudName": "AzureCloud",
    "id": "79526e60-e6bf-4461-a828-e0051650caaf",
    "isDefault": true,
    "name": "N/A(tenant level account)",
    "state": "Enabled",
    "tenantId": "79526e60-e6bf-4461-a828-e0051650caaf",
    "user": {
      "name": "juan.tous@arroyoconsulting.net",
      "type": "user"
    }
  },
  {
    "cloudName": "AzureCloud",
    "id": "931f624d-0a36-452b-8ed5-0063f9deaa6d",
    "isDefault": false,
    "name": "N/A(tenant level account)",
    "state": "Enabled",
    "tenantId": "931f624d-0a36-452b-8ed5-0063f9deaa6d",
    "user": {
      "name": "juan.tous@arroyoconsulting.net",
      "type": "user"
    }
  }
]
#####################


[
  {
    "cloudName": "AzureCloud",
    "homeTenantId": "931f624d-0a36-452b-8ed5-0063f9deaa6d",
    "id": "17b864fa-4fda-4b12-b357-b10487784c2b",
    "isDefault": true,
    "managedByTenants": [],
    "name": "Arroyo - PayAsYouGo",
    "state": "Enabled",
    "tenantId": "931f624d-0a36-452b-8ed5-0063f9deaa6d",
    "user": {
      "name": "juan.tous@arroyoconsulting.net",
      "type": "user"
    }
  }
]


####

{
  "id": "/subscriptions/17b864fa-4fda-4b12-b357-b10487784c2b/resourceGroups/arm-vscode",
  "location": "eastus",
  "managedBy": null,
  "name": "arm-vscode",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null,
  "type": "Microsoft.Resources/resourceGroups"
}


### Templates

{
  "id": "/subscriptions/17b864fa-4fda-4b12-b357-b10487784c2b/resourceGroups/myResourceGroup",
  "location": "centralus",
  "managedBy": null,
  "name": "myResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null,
  "type": "Microsoft.Resources/resourceGroups"
}


az deployment group create --name blanktemplate --resource-group myResourceGroup --template-file testmd



# Templates Json

App Service Plan[x]
app node [x]
despues el storage [x] ---falta probar
despues el kv [x] ----




