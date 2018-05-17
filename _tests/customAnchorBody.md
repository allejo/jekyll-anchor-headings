---
---

{% capture markdown %}
# Heading 1
{% endcapture %}
{% assign text = markdown | markdownify %}

{% capture anchor %}
    <span class="sr-only">Permalink to "%heading%"</span>
    <i class="fa fa-link" aria-hidden="true"></i>
{% endcapture %}

{% include linkify_headings.html html=text anchorBody=anchor %}

<!-- /// -->

<h1 id="heading-1">Heading 1 <a href="#heading-1">
    <span class="sr-only">Permalink to "Heading 1"</span>
    <i class="fa fa-link" aria-hidden="true"></i>
</a></h1>
