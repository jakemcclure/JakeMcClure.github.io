---
layout: page
title: Blog
description: Recent thoughts…
permalink: /blog/
siteNav: true
siteNav_order: 2
siteNav_label: blog
nav_icon_ligature: chrome_reader_mode
---
<ul class="post-list" id="featured-loop">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%-d %b • %Y" | upcase }}</span>

      <h2 class="post-list-title">
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
