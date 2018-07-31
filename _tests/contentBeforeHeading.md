---
# See: https://github.com/allejo/jekyll-anchor-headings/issues/3
---

{% capture markdown %}
This is a very short guide to using Travis CI with your GitHub hosted code repository.

## Prerequisites

To start using Travis CI, make sure you have all of the following:
{% endcapture %}
{% assign text = markdown | markdownify %}

<div>
{% include anchor_headings.html html=text %}
</div>

<!-- /// -->

<div>
    <p>This is a very short guide to using Travis CI with your GitHub hosted code repository.</p>
    <h2 id="prerequisites">Prerequisites <a href="#prerequisites"></a></h2>
    <p>To start using Travis CI, make sure you have all of the following:</p>
</div>
