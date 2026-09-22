---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am Guoguo Zhang, currently pursuing a PhD in Computer Science at Durham University, working on AI for audio and music, advised by Dr Brian Bemman. I received my Bachelor's degree in Music Performance from Sun Yat-sen University in 2024, and a Master of Music from the Royal Conservatoire of Scotland. I am broadly interested in AI, audio, music and therapy.

My CV can be found [here](/files/CV_Guoguo.pdf).

Publications
======

{% for post in site.publications reversed %}
**[{{ post.title }}]({{ base_path }}{{ post.url }})**  
{{ post.authors }}  
*{{ post.venue }}*, {{ post.date | date: "%Y" }}  
[\[Paper\]]({{ post.paperurl }}){% if post.code %} [\[Code\]]({{ post.code }}){% endif %}

{% endfor %}
