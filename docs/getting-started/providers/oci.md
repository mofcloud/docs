---
title: Oracle Cloud
description: Quickly configure Oracle Cloud and start analyzing cloud cost health.
---

System use FOCUS API from oracle cloud [object_storage:GetObject](https://docs.oracle.com/en-us/iaas/Content/Object/Tasks/managingobjects_topic-To_download_an_object_from_a_bucket.htm)
to fetch data.

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [ ] China
- [x] Global

### **Credential**
Please refer to official docs for credential: [Oracle Credential](https://docs.oracle.com/en-us/iaas/Content/Identity/Tasks/managingpasswordrules.htm)

The system only requires readable permissions. If the permissions are incomplete, data collection will be incomplete. You can select **Permission Table** to query permissions.

## Update account
Please refer to [Basic](basic.md)

## Features

| Features              | Description                                                                       |
|-----------------------|-----------------------------------------------------------------------------------|
| **Smart Bill**        | Group by**Service**、**Compartment**、**Region**、**Owner**、**Charge Type**、**Tags** |
| `Cost Explorer`       | :material-check:                                                                  |
| `Monthly Bill`        | :material-check:                                                                  |
| `Daily Bill`          | :material-check:                                                                  |
| `History Bill`        | :material-check:                                                                  |
| `Filters`             | :material-check:                                                                  |
| `Unit Cost Explorer`  | :material-check:                                                                  |
| `Resource Bill`       | :material-check:                                                                  |
| `Charge item & usage` | :material-check:                                                                  |
| `Mofis report`        | :material-check:                                                                  |
| `Download`            | :material-check:                                                                  |
| `Scheduled`           | :material-check:                                                                  |
| `Notification`        | :material-check:                                                                  |
| `Exchange`            | :material-check:                                                                  |
| `Server analysis`     | :material-check:                                                                  |
| **Data Sync**         |                                                                                   |
| `Manual`              | :material-check:                                                                  |
| `Auto`                | :material-check:                                                                  |
| **Tag Management**    | :material-check:                                                                  |
