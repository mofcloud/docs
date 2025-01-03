---
title: User Settings
description: User setting options, including changing password, subscribing, logging out, changing username, etc.
---

## Basic Info
- User name
- Default currency
- Lang

![Update user basic info](assets/setting/user-setting-basic.png)

## Subscription
![Update subscription](assets/setting/user-setting-sub.png)

## Report Subscription
Add message subscription webhook and scheduled push.

![Report Subscription](assets/setting/user-setting-notify.png)

### Report webhook
Supports **Enterprise WeChat group robots**, **DingTalk group robots**, **Lart Suit group robots**. For security reasons, the system supports the signature algorithm of group robots.

### Scheduled push
Users can push the following data to group robots at regular intervals.

- All cloud accounts (for the day, the month)
- Single cloud account (for the day, the month)
- Organizational structure (for the day, the month)

## Update password
If the user remembers the existing password, they can modify it directly. If the user does not remember the existing password, they can reset the password via email.

![Update password](assets/setting/user-setting-pass.png)

## Delete User
Once an account is cancelled, the system will immediately delete all user-related data. Including the following:

- Billing data
- Resource-related data
- Account-related data
- Message subscription-related data

![Delete User](assets/setting/user-setting-unregister.png)
