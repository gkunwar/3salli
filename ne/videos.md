---
layout: page
lang: ne
nav: videos
title: भिडियो
lede: मन्दिर, पूजा र समुदायसँग सम्बन्धित भिडियोहरू।
permalink: /ne/videos/
---

<div class="video-grid">
{% for video in site.data.videos %}
  <article class="video-item">
    <h2>{{ video.title_ne }}</h2>
    <p>{{ video.note_ne }}</p>
    {% include video-embed.html video=video %}
  </article>
{% endfor %}
</div>
