---
layout: default
title: Blog
ref: blog
permalink: /blog/
---

<div>
  <h2>Latest Posts</h2>

  {% assign posts_by_year = site.posts
    | group_by_exp: "post", "post.date | date: '%Y'"
    | sort: "name"
    | reverse
  %}

  {% for year_group in posts_by_year %}
    <h2>{{ year_group.name }}</h2>

    <ul class="post-list">
      {% assign year_posts = year_group.items | sort: "date" | reverse %}
      {% for post in year_posts %}
        {% assign date_format = site.cayman-blog.date_format | default: "%b %-d, %Y" %}
        <li>
          <span class="post-meta">{{ post.date | date: date_format }}</span>

          <h3>
            <a class="post-link"
               href="{{ post.url | absolute_url }}"
               title="{{ post.title | escape }}">
              {{ post.title | escape }}
            </a>
          </h3>

          {{ post.excerpt | markdownify | truncatewords: 30 }}
        </li>
      {% endfor %}
    </ul>
  {% endfor %}
</div>


