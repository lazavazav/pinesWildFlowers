---
title: "Blog"
description: "Learn how to help and to enhance your own yard to attract and foster native wildlife"
pagination:
  data: collections.blog
  size: 10
  alias: blog
---

<ul>
  {%- for post in collections.blog | reverse -%}
    <li>
      <h3><a href="{{ post.url | url }}">{{ post.data.title }}</a> | {{ post.date | readableDate }}</h3>
    </li>
  {%- endfor -%}
</ul>
