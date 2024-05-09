---
permalink: /about/
title: "About"
author_profile: false
---

{% for author in site.data.authors %}

**{{ author[1].name }}**
- {{ author[1].bio }}
{% for link in author[1].links %}
    - [{{ link.label }}]({{ link.url }})
{% endfor %}
{% endfor %}
