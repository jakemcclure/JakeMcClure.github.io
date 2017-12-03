---
title: Lab
description: My sandbox for mHealth ideas and pre-production clinical tools
nav_icon_ligature: healing
sitenav: true
sitenav_order: 3
featured_image:
featured_image_width:
featured_image_height:
featured_image_description:
---
{% for item in site.lab %}
<h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
<h4>{{ item.description }}</h4>
{% if item.featured_image %}
<amp-img alt="{{ item.featured_image_description }}"
  src="{{ item.featured_image }}"
  width="{{ item.featured_image_width }}"
  height="{{ item.featured_image_height }}"
  layout="responsive">
  <noscript>
    <img src="{{ item.featured_image }}" width="{{ item.featured_image_width }}"
    height="{{ item.featured_image_height }}" />
  </noscript>
</amp-img>
{% endif %}
{% endfor %}

### The Epic / Haiku / Cantu Wishlist
Ho, ho, ho …it's that time of year. What I wish Santa Judy Faulkner and her elves up in Madison would deliver.

[Add your suggestion to the wish list](mailto:holler@jakemcclure.net)
