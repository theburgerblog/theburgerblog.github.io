---
permalink: /about/
title: "About"
author_profile: true
---

{% for author in site.data.authors %}
![Image Description]({{ site.url }}{{ site.baseurl }}author.avatar)
- {{ author.name }}
- {{ author.bio }}
- {{ author.links }}
{% endfor %}
