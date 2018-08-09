---
title: Home
layout: default
---
# {{ site.github.project_title }}
## {{ page.title }}

{% for repository in site.github.public_repositories %}

<div class="columns mb-1">
  <div class="one-fourth column block-blue p-3 border">
    * [{{ repository.name }}]({{ repository.html_url }})
    {{ repository.description }}
  </div>
</div>
{% endfor %}
