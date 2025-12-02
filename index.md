---
layout: default
title: Home
---
<section class="hero">
  <h1>Hi — I'm Pramo</h1>
  <p>Welcome to my personal site. I write about projects, code, and a few ideas.</p>
  <p><a class="btn" href="/about">About</a> <a class="btn" href="/blog">Blog</a></p>
</section>

<section class="recent-posts">
  <h2>Recent posts</h2>
  <ul>
    {% for post in site.posts limit:5 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
  <p><a href="/blog">See all posts →</a></p>
</section>