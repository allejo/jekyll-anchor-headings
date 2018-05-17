---
---

{% capture markdown %}
# Heading 1
{% endcapture %}
{% assign text = markdown | markdownify %}

{% include linkify_headings.html html=text anchorTitle="Link to '%heading%'" %}

<!-- /// -->

<h1 id="heading-1">Heading 1 <a href="#heading-1" title="Link to 'Heading 1'"></a></h1>
