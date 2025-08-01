---
description: >-
  Steps to integrate our resources utilizing specific inventory features (e.g.,
  utility_kitchen)
---

# Installation for qb-inventory

Modify the resource

Replace or update your `qb-inventory` by following this commit or using the provided modified version.

{% embed url="https://github.com/qbcore-framework/qb-inventory/compare/main...MXC-PR:main" %}

### Run this SQL query using HeidiSQL or any other database viewer

```sql
ALTER TABLE inventories CHANGE COLUMN identifier identifier VARCHAR(100) NOT NULL
```
