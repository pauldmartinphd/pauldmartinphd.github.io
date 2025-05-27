---
title: "Blog"
layout: year-archive    # shows posts grouped by year
permalink: /blog/
author_profile: true
---

## Blog Posts



---

## Latest notes

{% if site.posts == empty %}
*No posts yet.*  
{% else %}
{% for post in site.posts limit:3 %}
* {{ post.date | date: "%b %d %Y" }} — **[{{ post.title }}]({{ post.url }})**
{% endfor %}
{% endif %}
