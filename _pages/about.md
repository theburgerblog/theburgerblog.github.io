---
permalink: /about/
title: "About"
author_profile: false
---
<div id="about-page" style="display: flex; flex-direction: row; justify-content: space-around;">
{% for author in site.data.authors %}

<div style="margin: 1rem; width: calc(50% - 2rem); border: 1px solid #000; padding: 1rem;">
  <img style="width: 100%;" src="{{ author[1].avatar }}" alt="Card image cap">
  <div>
    <h5>{{ author[1].name }}</h5>
    <p>{{ author[1].bio }}</p>
    <ul style="list-style: none; padding: 0;">
    {% for link in author[1].links %}
        <li>
            <a href="{{ link.url }}"><i class="{{ link.icon }}"></i> {{ link.label }}</a>
        </li>
    {% endfor %}
    </ul>
  </div>
</div>

{% endfor %}
</div>
