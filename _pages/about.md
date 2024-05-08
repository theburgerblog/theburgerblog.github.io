---
permalink: /about/
title: "About"
author_profile: true
---

<ul>
{% for member in site.data.authors %}
  <li>
    <a>
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>
