---
permalink: /about/
title: "About"
author_profile: false
---

{% for author in site.data.authors %}

**{{ author[0] }}**
- {{ author[1].bio }}
{% for link in author[1].links %}
    - [{{ link.icon }}]({{ link.url }})
{% endfor %}
{% endfor %}
