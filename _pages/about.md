---
permalink: /about/
title: "About"
author_profile: true
authors: site.data.authors
---
What is this???

title: {{page.title}}

{% for author in page.authors %}
- {{ author.name }} </br>
{% endfor %}

