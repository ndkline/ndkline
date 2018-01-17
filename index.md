---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

{% for project in site.projects %}
<h2>{{ project.title }}</h2>
<p>{{ project.description }}</p>
<p><a href="{{ project.url }}">{{ project.title }}</a></p>
{% endfor %}