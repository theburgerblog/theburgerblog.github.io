---
permalink: /about/
title: "About"
author_profile: true
authors: site.data.authors
---

{% for author in page.authors %}
- {{ author.name }} </br>
{% endfor %}

title: {{page.title}}
