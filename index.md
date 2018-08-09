---
title: Home
layout: default
---
# {{ site.github.project_title }}
## {{ page.title }}

{% for repository in site.github.public_repositories %}
  <div class="col-4 float-left border p-4">
    <a href="{{ repository.html_url }}">{{ repository.name }}</a>
    {{ repository.description }}
  </div>
{% endfor %}