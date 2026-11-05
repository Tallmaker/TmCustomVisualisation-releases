---
title: Template language
order: 20
---

# Template language

Use `{{Field}}` to show a value. `{{#each rows}}` repeats markup for rows, `{{#if value}}` shows markup conditionally, and `{{#group rows by Field}}` groups rows. Add `paged` to a row or group loop to show a pager.

Helpers format numbers, totals, shares, text and comparisons. `{{select Field}}` makes a value selectable, and `{{tooltip Field}}` shows a tooltip. Values are escaped and the safety filter checks the HTML and CSS.

See the [full template language guide](template-language-full.md).
