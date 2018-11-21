---
# See https://github.com/allejo/jekyll-anchor-headings/issues/5
---

{% capture markdown %}
# Heading 1

# Heading 2
{% endcapture %}
{% assign text = markdown | markdownify %}

<div>
{% include anchor_headings.html html=text bodyPrefix='<span class="after">' bodySuffix='</span>' %}
</div>

<!-- /// -->

<div>
<h1 id="heading-1"><span class="after">Heading 1 <a href="#heading-1"></a></span></h1>

<h1 id="heading-2"><span class="after">Heading 2 <a href="#heading-2"></a></span></h1>
</div>
