---
layout: page
title: Frequently asked questions
excerpt: "because our mind is always asking why this ? why that ?"
search_omit: true
image:
  feature: large_mer.jpg
  credit: kiwi
---
### You may have asked yourself...

<ul class="post-list">
{% for post in site.posts limit:10 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
