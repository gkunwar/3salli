---
layout: page
lang: ne
nav: videos
title: युट्युब भिडियो
lede: मन्दिर, पूजा र समुदायसँग सम्बन्धित भिडियोहरू।
permalink: /ne/videos/
---

<div class="video-grid">
{% for video in site.data.videos %}
  <article class="video-item">
    <h2>{{ video.title_ne }}</h2>
    <p>{{ video.note_ne }}</p>
    <div class="video-frame">
      <iframe
        src="https://www.youtube-nocookie.com/embed/{{ video.id }}"
        title="{{ video.title_ne }}"
        loading="lazy"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen></iframe>
    </div>
  </article>
{% endfor %}
</div>
