---
permalink: /about/
title: "About"
author_profile: true
---

{% for author in site.data.authors %}
- {{ author.name }} </br>
- {{ author.bio }} </br>
- {{ author.avatar }} </br>
{% endfor %}

Data:
{{site.data}}