---
permalink: /about/
title: "About"
author_profile: false
---

<div class="d-flex flex-wrap justify-content-around">
{% for author in site.data.authors %}

<div class="card m-2" style="width: 18rem;">
  <img class="card-img-top" src="{{ author[1].avatar }}" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">{{ author[1].name }}</h5>
    <p class="card-text">{{ author[1].bio }}</p>
    <ul class="list-group list-group-flush">
    {% for link in author[1].links %}
        <li class="list-group-item">
            <a href="{{ link.url }}"><i class="{{ link.icon }}"></i> {{ link.label }}</a>
        </li>
    {% endfor %}
    </ul>
  </div>
</div>

{% endfor %}
</div>
