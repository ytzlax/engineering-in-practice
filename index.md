---
layout: home
title: Home
---

# Welcome to Engineering in Practice 🚀

This is a space where I share my hands-on experiences building real-world projects, tackling technical challenges, and learning from the trenches of software and hardware development.

## Latest Posts

{% for post in site.posts %}
  <article class="post-preview">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }} • {{ post.reading_time }} min read</p>
    <p>{{ post.excerpt }}</p>
    <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
  </article>
{% endfor %}

---

## About

These posts document real experiences from real projects - the good, the bad, and the lessons learned. Each post dives into practical challenges, solutions, and insights from building things that matter.
