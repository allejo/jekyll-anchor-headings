---
---

{% capture markdown %}
# Heading 1
{% endcapture %}
{% assign text = markdown | markdownify %}

{% include linkify_headings.html html=text beforeHeading=true %}

<!-- /// -->

<h1 id="heading-1"><a href="#heading-1"></a> Heading 1</h1>
