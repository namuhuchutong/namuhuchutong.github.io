---
layout: default
title: test2
permallink: category/test2
---

{% assign posts = site.categories.test2 %}
{% assign sum = posts.size %}
<h1 class="post-title">{{ page.title }}<small> -- ({{posts.size }})</small></h1>

{% for post in posts %}
    {% include category.html %}
{% endfor %}