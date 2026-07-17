---
layout: page
lang: en
nav: videos
title: YouTube Videos
lede: Videos related to the temple, worship, and community life.
permalink: /en/videos/
---

<div class="video-grid">
{% for video in site.data.videos %}
  <article class="video-item">
    <h2>{{ video.title_en }}</h2>
    <p>{{ video.note_en }}</p>
    <div class="video-frame">
      <iframe
        src="https://www.youtube-nocookie.com/embed/{{ video.id }}"
        title="{{ video.title_en }}"
        loading="lazy"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen></iframe>
    </div>
  </article>
{% endfor %}
</div>
