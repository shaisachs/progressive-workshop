---
layout: page
title: Git repos
---

These repositories represent progressive tech projects. By and large they are open to contribution, so these are a great chance to find out what others are doing and to get your feet wet in the ecosystem!

<ul>

    {% for repo in site.gitrepos %}

<li><a href="{{ repo.repourl }}">{{ repo.title }}</a></li>

    {% endfor %}

</ul>
