---
permalink: /about/
title: "About"
author_profile: true
---

<ul>
{% for member in site.data.authors %}
      Name: {{ member.name }}
{% endfor %}
</ul>
