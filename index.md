---
#
# Here you can change the text shown in the Home page before the Latest Posts section.
#
# Edit jekyll-theme-simple-blog's home layout in _layouts instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home

header:
  image: /assets/img/home-header.jpg

ref: home
lang: en
---

Hello there. Welcome to my humble blog where I talk about the things I’ve learned the hard way in computer programming. I'll talk about things where I got some "aha" moment (like lambda) and also the stuff that I am currently learning.

<h2>Latest Articles</h2>
<div>&nbsp;</div>
{% include list-category-posts.html lang=page.lang category="articles" max=2 %}

---

<h2>Latest Projects</h2>
<div>&nbsp;</div>
{% include list-category-posts.html lang=page.lang category="projects" max=1 %}
