---
title: Data handling
order: 30
---

# Data handling

The object loads data in checked pages, up to 20,000 rows (5,000 by default). When not all rows are loaded, the object says so. Totals from Qlik stay exact even when only some rows are loaded.

The `paged` option on a row or group loop adds a pager. Helpers such as `sum`, `avg`, `min`, `max` and `count` use loaded rows; they stay empty when not all rows are loaded.
