---
title: AWS
description: Quickly configure AWS and start analyzing cloud cost health.
---

## Bill Types
We recommend enable **Data Exports** at AWS console which contains detail data and cheap while pulling since stored at S3.

Cost Explorer charges based on the number of requests, and frequent access may result in higher costs.

| Data Types              | Charge fees ? | Description                                                                                   |
|-------------------------|---------------|-----------------------------------------------------------------------------------------------|
| Cost Explorer           | ✅             | AWS charges based on the number of API calls (expensive).                                     |
| Legacy CUR              | ✅             | Supports resource billing, with bills stored in S3, incurring S3-related costs (inexpensive). |
| CUR 2.0 （Coming Soon）   | ✅             | Supports resource billing, with bills stored in S3, incurring S3-related costs (inexpensive). |
| FOCUS 1.0 （Coming Soon） | ✅             | Supports resource billing, with bills stored in S3, incurring S3-related costs (inexpensive). |


## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [x] China
- [x] Global

### **AK/SK**
Please refer to official docs for credential: [AWS Credential](https://docs.aws.amazon.com/zh_cn/IAM/latest/UserGuide/id_credentials_access-keys.html#Using_CreateAccessKey)

The system only requires readable permissions. If the permissions are incomplete, data collection will be incomplete. You can select **Permission Table** to query permissions.

### Data Export
> Support Legacy CUR now!

AWS does not enable data export by default. Please refer to [Creating Cost and Usage Reports in AWS](https://docs.aws.amazon.com/zh_cn/cur/latest/userguide/cur-create.html)，
Mof only requires the report name. If you have just enabled billing reports, AWS may take several hours to start syncing. Please be patient.

Impact of Options on the System:

- **Include Resource IDs:** Please select this; otherwise, resource-level billing cannot be viewed.
- **Split Cost Allocation Data:** No impact.
- **Auto-Refresh:** Please select this to ensure Mof retrieves the latest data each time.
- **Configure S3 Bucket:** No impact.
- **S3 Path Prefix:** No impact.
- **Time Granularity:** Select Daily or Hourly; Mof stores data monthly and daily.
- **Report Versioning:** Choose Overwrite Existing Reports.
- **Report Data Integration:** No impact.
- **Compression Type:** No impact.

## Update account
Please refer to [Basic](basic.md)

### Extensions
It can be modified. If the billing report name is changed, the system will synchronize data from the new report during the next sync.

## Features

| Features              | Description                                                       |
|-----------------------|-------------------------------------------------------------------|
| **Smart Bill**        | Group by**Service**、**Region**、**Owner**、**Charge Type**、**Tags** |
| `Cost Explorer`       | :material-check:                                                  |
| `Monthly Bill`        | :material-check:                                                  |
| `Daily Bill`          | :material-check:                                                  |
| `History Bill`        | :material-check:                                                  |
| `Filters`             | :material-check:                                                  |
| `Unit Cost Explorer`  | :material-check:                                                  |
| `Resource Bill`       | :material-check:                                                  |
| `Charge item & usage` | :material-check:                                                  |
| `Mofis report`        | :material-check:                                                  |
| `Download`            | :material-check:                                                  |
| `Scheduled`           | :material-check:                                                  |
| `Notification`        | :material-check:                                                  |
| `Exchange`            | :material-check:                                                  |
| `Server analysis`     | :material-check:                                                  |
| **Data Sync**         |                                                                   |
| `Manual`              | :material-check:                                                  |
| `Auto`                | :material-check:                                                  |
| **Tag Management**    | :material-check:                                                  |
