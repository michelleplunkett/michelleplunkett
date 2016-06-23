---
layout: page
permalink: /projects/
title: projects
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---

<ul class="post-list">
{% for poem in site.projects reversed %}
    <li>
        <h2><a class="project-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>