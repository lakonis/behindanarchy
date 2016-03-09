---
layout: default
title: Home
---

<div style="padding: 50px 30px 30px 30px; background-color:beige; margin-bottom:30px">
  <blockquote> Bienvenu sur le carnet de recherche {{ site.title }} consacré à l'étude du projet transmédia Anarchy.fr</blockquote>
  <a class="btn btn-default btn-sm" href="{{ site.github.url }}/about" title="About">
    <i class="fa fa-arrow-right"></i> Plus d'informations</a>

  <!-- <p><i class="fa fa-arrow-right"></i> <a href="{{ site.github.url }}/about" title="About">Plus d'informations</a></p> -->
</div>

<div class="home">

  <h1 class="page-heading">A lire sur <em>Behind Anarchy.fr</em> :</h1>

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
