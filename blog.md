---
layout: center-page
title: What's new?
permalink: /blog/
---
<ul class="post-list list-unstyled">
  {% for post in site.posts %}
    <li class="post-list-item">
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
          {{ post.title }}
          <small>
            {{ post.date | date: "%b %-d, %Y" }}
          </small>
        </a>
      </h2>
      <article>
        {{ post.content }}
      </article>
    </li>
  {% endfor %}
</ul>
