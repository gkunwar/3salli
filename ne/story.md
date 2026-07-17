---
layout: page
lang: ne
nav: story
title: मन्दिर कथा
lede: तीन सल्ली — तीन सल्ला र भगवती माताको आशीर्वादसँग जोडिएको थलो।
permalink: /ne/story/
---

{% assign story = site.data.story.ne %}

<p class="story-lead">{{ story.lead }}</p>

{% for section in story.sections %}
<section class="story-block">
  <h2>{{ section.title }}</h2>
  <p>{{ section.body }}</p>
</section>
{% endfor %}

<p><a class="btn btn-primary" href="{{ '/ne/history/' | relative_url }}">इतिहास हेर्नुहोस्</a></p>
