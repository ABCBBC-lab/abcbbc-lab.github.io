---
layout: page
permalink: /repositories/
title: repositories
description: These repositories contain code and data related to the research conducted at the ABCBBC Lab. They are open source and freely available for use and collaboration.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    <i class="fa-brands fa-github"></i>{% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
