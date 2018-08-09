---
title: Home
layout: default
---
# {{ site.github.project_title }}
## {{ page.title }}

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }} | {{ repository.description }}]({{ repository.html_url }})
{% endfor %}
