---
layout: page
title: Quick hits
---

<div class="container">
<section>

<p>This page is a pretty rough collection of ideas for improving the progressive tech ecosystem. Think you can improve on some of these ideas, or help flesh them out? Please <a href="/join-us">join us</a> or send us a <a href="https://github.com/shaisachs/progressive-workshop/pulls">pull request</a>!

<ul class="collection">
{% assign posts = site.quickhits %}
{% for post in posts %}
    <li class="collection-item avatar">

    <span class="title"><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></span>

    {{ post.content }}

</li>

{% endfor %}

</ul>  

</section>

</div>