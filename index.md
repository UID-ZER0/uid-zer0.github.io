---
layout: default
title: "uid-zer0"
---

<div class="container">
  <h1>Archive💾</h1>
  <p>Critical thoughts on the structures underneath modern life</p>

  <h2>Latest Articles</h2>

  <ul>
    {% for post in site.posts %}
      <li>
        <div class="card">
          <a href="{{ post.url }}">
            <h3>{{ post.title }}</h3>
          </a>
          <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
        </div>
      </li>
    {% endfor %}
  </ul>
</div>
