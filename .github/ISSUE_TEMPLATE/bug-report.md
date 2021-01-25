---
name: Bug Report
about: Something about your anchor links isn't being generated correctly
labels: bug

---

**Markdown Engine**

<!--
  Which markdown engine are you using? (e.g. kramdown, commonmark, redcarpet)
-->

Write here.

**My Markdown**

<!--
  Put the markdown you've written and is currently being fed into the
  `html` parameter. Only the headings are necessary and in the order
  you're using them.
-->

```markdown

```

**Snippet Usage**

<!--
  How are you using the anchor_headings.html include?

  Specify the parameters you're using in your {% include %}; that means
  values you're setting for `h_min`, `sanitize`, etc.
-->

```liquid
{% include anchor_headings.html html=content %}
```

**Expected HTML**

<!--
  The HTML of the anchor headings you expected to see
-->

```html

```

**Actual HTML**

<!--
  The HTML you got instead
-->

```html

```

**Notes**

<!--
  If there's anything else you'd like to say or would be useful, here's
  your chance to say it.
-->

Write here.
