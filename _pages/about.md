---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Guoguo Zhang, currently pursuing a PhD in Computer Science at Durham University, advised by Dr Brian Bemman, working on AI for audio and music. I received my Bachelor's degree in Music Performance from Sun Yat-sen University in 2024, and a Master of Music from the Royal Conservatoire of Scotland.
I am broadly interested in AI, audio, music and therapy.

My CV can be found [here](/files/CV_Guoguo.pdf).

## Publications

<style>
.pub {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  gap: 1.25em;
  margin-bottom: 2em;
}
.pub-thumb {
  flex: 0 0 240px;
  max-width: 240px;
}
.pub-thumb img {
  display: block;
  width: 100%;
  border-radius: 4px;
}
.pub-info {
  flex: 1 1 280px;
  min-width: 0;
  overflow-wrap: break-word;
}
.pub-info .pub-title {
  margin: 0 0 0.3em 0;
  font-size: 1.05em;
  line-height: 1.35;
  font-weight: bold;
}
.pub-info p {
  margin: 0 0 0.25em 0;
  font-size: 0.9em;
  line-height: 1.45;
}
.pub-authors {
  font-style: italic;
}
.pub-venue {
  color: #7a8288;
}
.pub-links a {
  margin-right: 0.5em;
  white-space: nowrap;
}
@media (max-width: 600px) {
  .pub {
    gap: 0.75em;
    margin-bottom: 1.5em;
  }
  .pub-thumb {
    flex-basis: 100%;
    max-width: 100%;
  }
  .pub-info .pub-title {
    font-size: 1em;
  }
  .pub-info p {
    font-size: 0.85em;
  }
  .pub-links a {
    display: inline-block;
    margin-top: 0.15em;
  }
}
</style>

<div class="pub-list">
{% for post in site.publications reversed %}<div class="pub">
{% if post.thumbnail %}<div class="pub-thumb"><img src="{{ post.thumbnail | prepend: '/images/' }}" alt="{{ post.title }}" /></div>
{% endif %}<div class="pub-info">
<div class="pub-title">{{ post.title }}</div>
<p class="pub-authors">{{ post.authors | markdownify | remove: '<p>' | remove: '</p>' }}</p>
<p class="pub-venue">{{ post.venue }}, {{ post.date | date: "%Y" }}</p>
<p class="pub-links">{% if post.paperurl %}<a href="{{ post.paperurl }}">[Paper]</a>{% endif %}{% if post.code %}<a href="{{ post.code }}">[Code]</a>{% endif %}</p>
</div>
</div>
{% endfor %}</div>
