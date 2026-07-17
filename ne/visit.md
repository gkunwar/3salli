---
layout: page
lang: ne
nav: visit
title: कसरी पुग्ने
lede: लुम्बिनी प्रदेशका प्रमुख शहरहरूबाट अर्घाखाँची, मलारानी–२, गर्छास्थित मन्दिर पुग्ने बाटो।
permalink: /ne/visit/
---

{% assign t = site.data.strings.ne %}

<p><strong>{{ t.location }}</strong> · {{ t.province }}</p>

<div class="route-list">
{% for route in site.data.directions %}
  <article class="route">
    <h2>{{ route.city_ne }} {{ t.visit_from }}</h2>
    <p class="route-duration">{{ route.duration_ne }}</p>
    <ol>
      {% for step in route.steps_ne %}
      <li>{{ step }}</li>
      {% endfor %}
    </ol>
    <p class="route-tip"><strong>{{ t.visit_tip_title }}:</strong> {{ route.tip_ne }}</p>
  </article>
{% endfor %}
</div>
