---
permalink: /about/
title: "About"
author_profile: false
---

{% for author in site.data.authors %}
![Image Description]({{ site.url }}{{ site.baseurl }}author.avatar)

**{{ author.name }}**
- {{ author.bio }}
{% for link in author.links %}
    - [{{ link.icon }}]({{ link.url }})
{% endfor %}
{% endfor %}

{{ site.url }}

{{ site.baseurl }}

{{ site.data.authors }}

{{ site.data.authors.florian }}
