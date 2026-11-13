---
title: Requirements and limits
order: 40
---

# Requirements

Tested on Qlik Cloud with Chrome. Other browsers are not yet tested. Image sources must be allowed by the tenant's content-source policy, and fonts must already be available in the browser. Create app variables before using them; absent-variable behavior still needs hosted verification.

The Tallmaker license is supplied through the separate license extension issued for your tenant. This visualization contains no license. License attention does not block rendering or interaction.

## Rows, paging and totals

Maximum rows to load defaults to 5,000 and can be set from 100 to 200,000, subject to a two-million-cell cap. Data loads in checked pages so rows from different selections are not mixed. A notice identifies incomplete or capped data. Qlik grand totals stay exact; helpers that require all rows do not calculate misleading summaries from a capped dataset.

A paged loop shows 25 rows per page by default, configurable from 5 to 500. An unpaged loop that would draw more than 20,000 rows shows a notice instead. Large loads take more time and memory: prefer paging or aggregation. Native sorting, calculation conditions, View data and Export data are supported.

## Export and snapshots

Image and PDF export of this object are unsupported. Qlik's reporting service leaves third-party extensions out of sheet PDFs and reports. Story snapshots can be created on Qlik Cloud; playback in a story is not yet verified.

## Design responsibility

Keep SVG aspect ratios intact and reserve space for labels. Viewport helpers can adapt templates to the available size; author scripts receive size and resize events. Native styling approximates the app theme. Custom templates remain the author's responsibility for layout, data meaning and accessibility.

Use template selection and tooltip helpers to provide keyboard interaction. Selections wait for Qlik's pending-selection confirmation. Sheet links work in the Qlik client outside edit mode and are hidden in snapshots. A custom view should be checked at the sizes and with the data its viewers will use.
