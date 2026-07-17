---
layout: page
lang: en
nav: videos
title: Videos
lede: Videos related to the temple, worship, and community life.
permalink: /en/videos/
---

<div class="video-grid">
{% for video in site.data.videos %}
  <article class="video-item">
    <h2>{{ video.title_en }}</h2>
    <p>{{ video.note_en }}</p>
    {% include video-embed.html video=video %}
  </article>
{% endfor %}
</div>
