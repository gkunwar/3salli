---
layout: page
lang: en
nav: visit
title: How to Reach
lede: Routes from major cities of Lumbini Province to the temple at Arghakhanchi, Malarani-2, Garchha.
permalink: /en/visit/
---

{% assign t = site.data.strings.en %}

<p><strong>{{ t.location }}</strong> · {{ t.province }}</p>

<div class="route-list">
{% for route in site.data.directions %}
  <article class="route">
    <h2>{{ t.visit_from }} {{ route.city_en }}</h2>
    <p class="route-duration">{{ route.duration_en }}</p>
    <ol>
      {% for step in route.steps_en %}
      <li>{{ step }}</li>
      {% endfor %}
    </ol>
    <p class="route-tip"><strong>{{ t.visit_tip_title }}:</strong> {{ route.tip_en }}</p>
  </article>
{% endfor %}
</div>

{% include map.html %}
