---
layout: page
title: Idea lab
---

<div class="container last-post">
<section>

<ul class="collection">
{% assign posts = site.posts | where: 'category', 'idealab' %}
{% for post in posts %}
    <li class="collection-item avatar">

    {% assign date_format = site.minima.date_format | default: "%d %b" %}
    <div class="date-post">{{ post.date | date: date_format }}</div>
    <span class="title"><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></span>
    <p>
    {{ post.content | strip_html | truncatewords: 10 }}
    </p>
    <a href="{{ post.url | relative_url }}" class="secondary-content"><i class="material-icons">navigate_next</i></a>

</li>

{% endfor %}

</ul>

<p>See our <a href="/quick-hits">Quick hits</a> page for more ideas that we haven't yet fully fleshed out, and please feel free to contribute!</p>

</section>

</div>