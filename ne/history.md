---
layout: page
lang: ne
nav: history
title: मन्दिरको इतिहास
lede: तीन सल्ली भागवती मन्दिरको यात्रा — पुरानो थलोदेखि हालको संरचना र नयाँ योजनासम्म।
permalink: /ne/history/
---

{% assign t = site.data.strings.ne %}

<div class="history-list">
{% for era in site.data.history %}
  <article class="history-item">
    <div>
      <p class="history-meta">{{ era.year_ne }} · {{ t[era.era_key] }}</p>
      <h2>{{ era.title_ne }}</h2>
      <p>{{ era.body_ne }}</p>
    </div>
    <figure class="history-media">
      <img src="{{ era.image | relative_url }}" alt="{{ era.title_ne }}" width="1200" height="750">
    </figure>
  </article>
{% endfor %}
</div>
