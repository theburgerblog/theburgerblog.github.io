---
permalink: /about/
title: "About"
author_profile: true
---

{% for author in site.data.authors %}
- {{ author }}
- {{ author.name }} </br>
- {{ author.bio }} </br>
- {{ author.avatar }} </br>
{% endfor %}

Data
{{ site.data }}

Authors
{{ site.data.authors }}

Author1
{{ site.data.authors[0] }}

Navigation
{{ site.data.navigation }}
