---
layout: page
lang: en
nav: history
title: Temple History
lede: From the old shrine to the present structure and plans for the new temple.
permalink: /en/history/
---

{% assign t = site.data.strings.en %}

<div class="history-list">
{% for era in site.data.history %}
  <article class="history-item">
    <div>
      <p class="history-meta">{{ era.year_en }} · {{ t[era.era_key] }}</p>
      <h2>{{ era.title_en }}</h2>
      <p>{{ era.body_en }}</p>
    </div>
    <figure class="history-media">
      <img src="{{ era.image | relative_url }}" alt="{{ era.title_en }}" width="1200" height="750">
    </figure>
  </article>
{% endfor %}
</div>
