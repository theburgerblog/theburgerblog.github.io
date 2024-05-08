---
permalink: /about/
title: "About"
author_profile: true
---

{% assign authors = site.data.authors %}

## Authors

{% for author in authors %}
- Name: {{ author.name }}
    Bio: {{ author.bio }}
{% endfor %}