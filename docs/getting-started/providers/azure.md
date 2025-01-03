---
title: Azure
description: Quickly configure Azure and start analyzing cloud cost health.
---

The system will read billing-related data through the service principal.

## Preparation
Install Azure CLI (if you already have a service principal, please skip this step)

If you don't have a service principal, please follow the steps below to create one. Alternatively, you can create it in the Azure portal; for the steps, refer to the official documentation.

### 1.Create Azure Service Principal
Run bellow commands.

Please copy appId, tenant, password which are needed by system.

```shell
az ad sp create-for-rbac -n "mofcloud"
```

### 2. Add Permissions
You can assign the READ permissions of the Billing account or Management Group to the service principal.

Run the following command (Billing account or Management Group ID can be obtained from the portal):

```shell
az role assignment create --assignee <SERVICE_PRINCIPAL_APP_ID> --role Reader --scope "/providers/Microsoft.Management/managementGroups/<MANAGEMENT_GROUP_ID>"
```

OR

```shell
az role assignment create --assignee <SERVICE_PRINCIPAL_APP_ID> --role Reader --scope "/providers/Microsoft.Management/managementGroups/<MANAGEMENT_GROUP_ID>"
```

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [ ] China
- [x] Global

### **Credentials**
Fill in the key information created in Step 1.

The system only requires read-only permissions. If the permissions are incomplete, it will result in incomplete data collection. You can refer to the permissions table to check the required permissions.

## Update account
Please refer to [Basic](basic.md)

## Features

| Features              | Description                                                                                           |
|-----------------------|-------------------------------------------------------------------------------------------------------|
| **Smart Bill**        | Group by**Service**、**Resource group**、**Subscription**、**Region**、**Owner**、**Charge Type**、**Tags** |
| `Cost Explorer`       | :material-check:                                                                                      |
| `Monthly Bill`        | :material-check:                                                                                      |
| `Daily Bill`          | :material-check:                                                                                      |
| `History Bill`        | :material-check:                                                                                      |
| `Filters`             | :material-check:                                                                                      |
| `Unit Cost Explorer`  | :material-check:                                                                                      |
| `Resource Bill`       | :material-check:                                                                                      |
| `Charge item & usage` | :material-check:                                                                                      |
| `Mofis report`        | :material-check:                                                                                      |
| `Download`            | :material-check:                                                                                      |
| `Scheduled`           | :material-check:                                                                                      |
| `Notification`        | :material-check:                                                                                      |
| `Exchange`            | :material-check:                                                                                      |
| `Server analysis`     | :material-check:                                                                                      |
| **Data Sync**         |                                                                                                       |
| `Manual`              | :material-check:                                                                                      |
| `Auto`                | :material-check:                                                                                      |
| **Tag Management**    | :material-check:                                                                                      |
