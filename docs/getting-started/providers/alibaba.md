---
title: Alibaba Cloud
description: Quickly configure Alibaba Cloud and start analyzing cloud cost health.
---

System use Alibaba Cloud API [DescribeInstanceBill](https://help.aliyun.com/document_detail/473030.htm) to fetch data.

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [x] China
- [x] Global

### **AK/SK**
Please refer to official docs for credential: [AWS Credential](https://help.aliyun.com/document_detail/268244.html)

The system only requires readable permissions. If the permissions are incomplete, data collection will be incomplete. You can select **Permission Table** to query permissions.

## Update account
Please refer to [Basic](basic.md)

## Features

| Features              | Description                                                                     |
|-----------------------|---------------------------------------------------------------------------------|
| **Smart Bill**        | Group by**Service**、**Cost Unit**、**Region**、**Owner**、**Charge Type**、**Tags** |
| `Cost Explorer`       | :material-check:                                                                |
| `Monthly Bill`        | :material-check:                                                                |
| `Daily Bill`          | :material-check:                                                                |
| `History Bill`        | :material-check:                                                                |
| `Filters`             | :material-check:                                                                |
| `Unit Cost Explorer`  | :material-check:                                                                |
| `Resource Bill`       | :material-check:                                                                |
| `Charge item & usage` | :material-check:                                                                |
| `Mofis report`        | :material-check:                                                                |
| `Download`            | :material-check:                                                                |
| `Scheduled`           | :material-check:                                                                |
| `Notification`        | :material-check:                                                                |
| `Exchange`            | :material-check:                                                                |
| `Server analysis`     | :material-check:                                                                |
| **Data Sync**         |                                                                                 |
| `Manual`              | :material-check:                                                                |
| `Auto`                | :material-check:                                                                |
| **Tag Management**    | :material-check:                                                                |
