---
layout: page
title: Main page
---

Hello, surfer!

Blog Posts aka notes.

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

    {{post.excerpt | markdownify}}
    [read more]({{ post.url }})
{% endfor %}