---
layout: page
title: Home
tagline: Supporting tagline
---
{% include JB/setup %}

## Últimos posts

<ul class="posts">
  {% for post in site.posts %}

  	{% if post.draft != true %}
    	<li>
          <span class="date">{{ post.date | date_to_string }}</span>
          <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}

  {% endfor %}
</ul>
