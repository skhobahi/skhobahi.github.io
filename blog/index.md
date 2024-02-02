---
layout: page
title: Blog
description: Notes of Shahin Khobahi
permalink: /blog/
---

Here you can find my experiments, thoughts, and analyses on a variety of topics.

<ul>
  {% for post in site.categories.post %}
    <li>
        <span>{{ post.date | date_to_string }}</span> » {% if post.highlight %}&starf; {% endif %}<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title | truncate:72 }}</a>
    </li>
  {% endfor %}
</ul>
