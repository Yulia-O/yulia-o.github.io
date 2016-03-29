---
layout 		: page
title 		: Blog Archive
description	: Blog posts archive
tags        : [blog]
icon: comments
---

<ul>
  {% for post in site.posts %}
    <li>
      <large><a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a></large>
      <small><i><time> {{ post.date | date: "%B %-d, %Y" }} </time></i></small>
    </li>
  {% endfor %}
</ul>
