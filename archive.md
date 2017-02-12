---
layout: page
title: Archief
---

{% for post in site.posts %}
{% assign author = site.data.people[post.author] %}
  * {{ post.date | date_to_string }} » [ {{ post.title }} ]({{ post.url }}){% if author != null %} - <small> {{author.name}}</small>{% endif %}
{% endfor %}