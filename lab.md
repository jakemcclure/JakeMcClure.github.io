---
title: Lab
description: My sandbox for mHealth ideas and pre-production clinical tools
siteNav: true
siteNav_order: 3
siteNav_label: lab
nav_icon_ligature: healing
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
