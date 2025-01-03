---
title: Showback
description: Create custom showback units and allocate cloud account bill to them.
---

In a multi-cloud environment, cost allocation has always been a problem. Users can use the **Cost Allocation** function to easily allocate cloud account costs to custom collections.

## 1.Create units
A unit is a structure similar to a file system. Users can create tree-like units and then allocate cloud account bills to the units.

Units can have the same name, but this is not recommended.

![Create units](assets/showback/create-unit.png)

## 2.Select month
The allocation rules are different every month because the allocation ratios of shared resource types (such as K8s) will be different.

![Select month](assets/showback/create-unit.png)

## 3.Bind cloud account
Select the cloud account and select the classification dimension. Users need to allocate different classifications to units.

![Bind cloud account](assets/showback/bind-account.png)

## 4.Allocate
Select the groups under the cloud account and allocate it to the created unit.

![Allocate](assets/showback/map-group.png)

## 5.Save ruleset
Be sure to save the allocation rules.

![Save ruleset](assets/showback/save-ruleset.png)

## 5.Check showback
![Check showback](assets/showback/showback.png)

