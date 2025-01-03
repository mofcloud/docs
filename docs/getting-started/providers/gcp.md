---
title: Google Cloud
description: Quickly configure Google Cloud and start analyzing cloud cost health.
---

The system will read Google Cloud billing-related data through the service account.

## Preparation
You need to export Cloud Billing data to BigQuery. If you have not yet exported Cloud Billing data to BigQuery, it is recommended to create a dedicated project to host the Cloud Billing data for better management of your billing data. 
For detailed steps, refer to the Google Cloud Official Documentation - [Export Cloud Billing Data to BigQuery](https://cloud.google.com/billing/docs/how-to/export-data-bigquery).

Please follow these steps:

1. Create a new project to host the Cloud Billing export data.
2. Create a BigQuery dataset to store the Cloud Billing export data.
3. Enable Cloud Billing export and export the data to the BigQuery dataset you created.

#### 1.Create Service Account
Create a service account in the project that hosts the Cloud Billing data.
When creating the service account, grant it the "BigQuery Job User" role and the "Cloud Asset Viewer" role for the project.
After the service account is created, generate a JSON format key for subsequent configuration.


#### 2.Add BigQuery Permissions
Navigate to BigQuery. Ensure that you are in the project hosting the Cloud Billing data.
In the "Explorer" panel, find the Cloud Billing dataset, click the vertical three dots (⋮) next to the name, and then click "Share." On the right, click "+ Add Principal."
Enter the service account created earlier. Assign the "BigQuery Data Viewer" role and save.


#### 3.Enable Cloud Asset API
If you have not enabled the Cloud Asset API, navigate to API & Services, click "+ Enable APIs and Services".
Search for "Cloud Asset API", go to the API details page, and click Enable.

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [ ] China
- [x] Global

### Credential
The system only requires read-only permissions. If the permissions are incomplete, it will result in incomplete data collection. 
You can choose **Test Account Permissions** to check the required permissions.

- **Service account key (JSON format)**

    Enter the JSON format key of the service account.

- **BigQuery Dataset name**

    Enter the name of the BigQuery dataset where the Cloud Billing data is stored.

- **BigQuery Table name**

    Enter the name of the BigQuery dataset table where the Cloud Billing data is stored.


## Update account
Please refer to [Basic](basic.md)

### Extension
Can be modified. If the BigQuery-related names are changed, the system will synchronize data from the new dataset during the next sync.

## Features

| Features              | Description                                                                     |
|-----------------------|---------------------------------------------------------------------------------|
| **Smart Bill**        | Group by**Service**、**Region**、**Owner**、**Charge Type**、**Tags** |
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
