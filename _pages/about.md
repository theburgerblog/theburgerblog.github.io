---
permalink: /about/
title: "About"
author_profile: true
---

{% for author in site.data.authors %}
![Image Description]({{ site.url }}{{ site.baseurl }}author.avatar)
**{{ author.name }}**
- {{ author.bio }}
{% for link in author.links %}
    - [{{ link.icon }}]({{ link.url }})
{% endfor %}
{% endfor %}

