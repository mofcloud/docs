---
title: Cloudflare
description: Quickly configure Cloudflare and start analyzing cloud cost health.
---

The system uses Cloudflare GraphQL to retrieve CDN usage data. Users need to configure the CDN pricing information signed with Cloudflare in order to calculate the billing data.

In the future, we will support retrieving billing data via API.

## Partial support
> Only **CDN** is supported now.

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [ ] China
- [x] Global

### **Credential**
Please refer to official docs for credential: [Cloudflare Credential](https://developers.cloudflare.com/fundamentals/api/get-started/create-token/)

The system only requires readable permissions. If the permissions are incomplete, data collection will be incomplete. You can select **Permission Table** to query permissions.

### **Extension**
If the minimum guaranteed traffic and minimum guaranteed cost are provided, Mof will first check if the usage is within the guaranteed range. If it exceeds, the cost will be calculated using the CDN unit price.

If the minimum guaranteed traffic and minimum guaranteed cost are not provided, Mof will calculate the cost using the CDN unit price.

| Options                            | Description                                                                                                                                      |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| CDN Price(USD/GB)                  | CDN traffic unit price. If the minimum guaranteed traffic and minimum guaranteed price are provided, this price will be the overflow unit price. |
| CDN minimum guaranteed traffic(GB) | If you have signed a minimum guarantee with Cloudflare, please enter the minimum guaranteed traffic; otherwise, enter 0.                         |
| CDN minimum guaranteed price(美元)   | If you have signed a minimum guarantee with Cloudflare, please enter the minimum guaranteed traffic; otherwise, enter 0.                         |
| Price start month                  | Contract start month                                                                                                                             |
| Price end month                    | Contract start month                                                                                                                                            |

## Update account
Please refer to [Basic](basic.md)

### **Extension**
Editable。

## Features

| Features              | Description          |
|-----------------------|----------------------|
| **Smart Bill**        | Groups not supported |
| `Cost Explorer`       | :material-check:     |
| `Monthly Bill`        | :material-check:     |
| `Daily Bill`          | :material-check:     |
| `History Bill`        | :material-check:     |
| `Filters`             |                      |
| `Unit Cost Explorer`  |                      |
| `Resource Bill`       |                      |
| `Charge item & usage` |                      |
| `Mofis report`        | :material-check:     |
| `Download`            | :material-check:     |
| `Scheduled`           | :material-check:     |
| `Notification`        | :material-check:     |
| `Exchange`            | :material-check:     |
| `Server analysis`     |                      |
| **Data Sync**         |                      |
| `Manual`              | :material-check:     |
| `Auto`                | :material-check:     |
| **Tag Management**    |                      |
