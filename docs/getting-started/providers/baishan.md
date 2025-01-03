---
title: Baishan Cloud
description: Quickly configure Baishan Cloud and start analyzing cloud cost health.
---

System use [chormedp](https://github.com/chromedp/chromedp) login to console and fetching CDN data.

User needs to configure the CDN pricing information signed with Baishan Cloud in order to calculate the billing data.

## Partial support
> Only **CDN** is supported now.

## Add account
### **Basic info**
Please refer to [Basic](basic.md)

### **Region**
Please select the corresponding region according to the account. **Editable**

- [x] China
- [ ] Global

### **Credential**
Please enter [Baishan console](https://uc.portal.baishancloud.com/home.html#/login) login email and password
Only billing data will be collected. Mof won't do any **write** operation.

### **Extension**
| Option              | Description          |
|---------------------|----------------------|
| CDN Price (Yuan/MB) | CDN price by traffic |
| Start Month         | Contract start month |
| End Month           | Contract end month   |

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
