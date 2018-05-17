---
---

{% capture markdown %}
# Heading 1

## Heading 1.1

## Heading 1.2

# Heading 2
{% endcapture %}
{% assign text = markdown | markdownify %}

<div>
{% include linkify_headings.html html=text %}
</div>

<!-- /// -->

<div>
<h1 id="heading-1">Heading 1 <a href="#heading-1"></a></h1>

<h2 id="heading-11">Heading 1.1 <a href="#heading-11"></a></h2>

<h2 id="heading-12">Heading 1.2 <a href="#heading-12"></a></h2>

<h1 id="heading-2">Heading 2 <a href="#heading-2"></a></h1>
</div>
