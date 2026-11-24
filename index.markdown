---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Home
---

I am a post-doctoral researcher, currently in the PESTO team at Inria Nancy.

{% assign sections = site.sections | sort: "order" %}
{% for section in sections %}
<section id="{{ section.slug }}">
  <h2>{{ section.title }}</h2>
  {{ section.content | markdownify }}
</section>
{% endfor %}
