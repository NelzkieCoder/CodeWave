---
layout: category
title: Tags
tagtitle: Tags
tagline: These are the tags associated with my articles post

permalink: /Tag.html
header:
  image: /assets/patterns/new_year_background.png
ref: tags
lang: en
order: 3
category: Tags
---


<br />
{% for tag in site.tags %}


<div style="display:inline;"><a href="{{ site.baseurl }}/tags/{{tag[0]}}" class="tagbig">{{ tag[0]  }}</a></div>


<!-- <div style="display:inline;"><a href="{{ site.baseurl }}/tags/{{tag[0]}}" class="tagbig">{{ tag[0]  }}</a></div>  -->

{% endfor %}
