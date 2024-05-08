---
permalink: /about/
title: "About"
author_profile: true
---
What is this???

title: {{page.title}}

{% for author in psite.data.authors %}
- {{ author.name }} </br>
{% endfor %}

Data:
{{site.data}}