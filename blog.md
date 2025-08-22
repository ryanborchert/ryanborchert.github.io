---
layout: default
title: "Blog - Engineering Leadership & Technical Insights"
description: "Technical insights and leadership lessons from an engineering director"
permalink: /blog/
---

# Blog

Thoughts on engineering leadership, technical decision-making, and lessons learned from building and scaling software teams.

{% for post in site.posts %}
  <article style="margin-bottom: 2em; padding-bottom: 1em; border-bottom: 1px solid #eee;">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p style="color: #666; font-size: 0.9em;">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.description | default: post.excerpt }}</p>
    <a href="{{ post.url }}">Read more →</a>
  </article>
{% endfor %}