---
layout: default
---

{% for repository in site.github.public_repositories %}
  * # [{{ repository.name }}]({{ repository.html_url }})
    {% if repository.description %}
        {{ repository.description }}
    {% endif %}
    {% if repository.open_issues_count %}
        Open issues: {{ repository.open_issues_count }}
    {% endif %}

{% endfor %}

