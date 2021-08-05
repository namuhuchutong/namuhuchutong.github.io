---
layout: default
title: test1
permallink: category/test1
---
{% assign posts = site.categories.test1 %}
{% assign sum = posts.size %}
<h1 class="post-title">{{ page.title }}<small> -- ({{posts.size }})</small></h1>
{% for post in posts %}
    {% include category.html %}
{% endfor %}