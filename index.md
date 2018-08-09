---
title: Home
layout: default
---
# {{ site.github.project_title }}
## {{ page.title }}

{% for repository in site.github.public_repositories %}
  <div class="col-4 float-left p-2">

    <div class="Box">
      <div class="Box-header">
        <h3 class="Box-title">
            <a href="{{ repository.html_url }}">{{ repository.name }}</a>
        </h3>
      </div>
      <div class="Box-body">
        {{ repository.description }}
      </div>
    </div>
    
  </div>
{% endfor %}