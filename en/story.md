---
layout: page
lang: en
nav: story
title: Temple Story
lede: Teen Salli — a shrine woven with pine hills and the blessing of Bhagwati Mata.
permalink: /en/story/
---

{% assign story = site.data.story.en %}

<p class="story-lead">{{ story.lead }}</p>

{% for section in story.sections %}
<section class="story-block">
  <h2>{{ section.title }}</h2>
  <p>{{ section.body }}</p>
</section>
{% endfor %}

<p><a class="btn btn-primary" href="{{ '/en/history/' | relative_url }}">Explore the history</a></p>
