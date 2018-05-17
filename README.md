# Jekyll Pure Liquid Heading Anchors

[![Build Status](https://travis-ci.com/allejo/jekyll-anchor-headings.svg?branch=master)](https://travis-ci.com/allejo/jekyll-anchor-headings)

> :warning: :construction: :construction: :construction: :warning:
>
> This is an incredibly young project and has not had much exposure to the real world. So I'd like to ask that if you're reading this, please help me out in one (or all) of the following ways:
>
> - Report any bugs you may find
> - Build your website with `--profile` and send me stats on your total build time, the amount of time this snippet takes, and the amount of times this snippet is used in your site
> - Star the project and share it with your friends!
>
> I'd like to tag a version **1.0.0**, but would like some real world testing to be done first.

GitHub Pages can't run custom Jekyll plug-ins so when generating anchors for your headings (i.e. `h1` - `h6`), you're stuck with JavaScript solutions that will inject anchors. But what if your users don't have JavaScript enabled on their browsers? If you're building a static website, might as well inject your anchors.

As a part of my "Pure Liquid" series of Jekyll snippets, here is a Liquid snippet that will modify your generated HTML to inject anchors.

## Usage

Alright, so how do you use it?

1. Download the latest [`anchor_headings.html`](_includes/anchor_headings.html)
2. Toss that file in your `_includes` folder
3. Where you typically would put `{{ content }}` in your layout, you would instead use this Liquid tag to output your page's content:

   ```liquid
   {% include anchor_headings.html html=content %}
   ```

## Parameters

This snippet is highly customizable. Here are the available parameters to change the behavior of the snippet.

| Parameter       |  Type  | Default | Description |
| --------------  | :----: | :-----: | ----------- |
| `html`          | string | <sup>*</sup> | the HTML of compiled markdown generated by kramdown in Jekyll |
| `beforeHeading` | bool   | false | Set to true if the anchor should be placed _before_ the heading's content |
| `anchorBody`    | string | ''    |  The content that will be placed inside the anchor; the `%heading%` placeholder is available
| `anchorClass`   | string | ''    |  The class(es) that will be used for each anchor. Separate multiple classes with a space
| `anchorTitle`   | string | ''    |  The `title` attribute that will be used for anchors; the `%heading%` placeholder is available

<sup>*</sup> This is a required parameter

## License

This snippet may be redistributed under the [MIT](LICENSE.md) license.