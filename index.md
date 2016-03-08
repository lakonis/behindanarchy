---
layout: default
title: Home
---

<div style="padding: 50px 30px 30px 30px; background-color:beige; margin-bottom:30px">
  <blockquote> {{ site.title }} est un carnet de recherche sur le projet transmédia Anarchy.fr</blockquote>
  <p><i class="fa fa-arrow-right"></i> Check <a href="{{ site.github.url }}/about)" title="About">About</a> and come back soon for brilliant content.</p>
</div>

<div class="home">

  <h1 class="page-heading">A lire sur Behind Anarchy :</h1>
  
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%-d %b, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.github.url }}">{{ post.title }}</a>
        </h2>
        {{ post.excerpt }}
        <hr>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.github.url }}">via RSS</a></p>

</div>
