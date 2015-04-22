---
layout: page
title: Brainmade Software Engineering - Unique, Intelligent, Stylish.
---

Hello, surfer!

Here is my Blog Posts AKA notes.

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

    {{post.excerpt | markdownify}}
    [read more]({{ post.url }})
{% endfor %}