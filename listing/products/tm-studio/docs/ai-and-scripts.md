---
title: AI and author scripts
order: 30
---

# Ask an AI assistant for a template

Describe the object you want under AI assistant and choose Copy prompt for AI. The prompt includes the data shape, your current template, template rules and independent working HTML/CSS and script examples. Paste it into your chosen AI assistant, then paste the complete reply back into the panel and choose Apply pasted reply.

Sample rows are excluded by default. Include sample rows only if the object's data may be shared with that tool: those rows leave Qlik when you paste the prompt. Review the generated layout, calculations and interactions. A changed script stays off until you review and enable it.

## Optional author script

Run author script is off by default. Enable it for JavaScript drawing, animation or interaction inside a sealed frame. The script API supplies this object's data, theme, size, lifecycle events and controlled selection requests. It cannot directly access Qlik, the rest of the sheet or the network.

Only use scripts you trust. A script can expose the data it receives through its output. Scripts run on Qlik Cloud; where site security blocks them, the HTML/CSS template displays without the script. Other Qlik sites and browsers are not yet tested.

## Template security

Values are escaped, HTML is sanitized, and CSS is filtered and scoped to the object. Custom design tokens accept only known names and validated values. Author scripts use the separate frame described above. These boundaries do not replace the author's responsibility to check the meaning, accessibility and suitability of a custom view.
