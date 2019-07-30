---
layout: default
title: Blog
permalink: /blog/
---
<div class="container blog">
  <header>
  </header>
  <section class="section latest-posts">
    <h2>Latest posts</h2>
    <div class="posts-container">
      {% for post in site.posts %}
        {% include postcard.html %}        
      {% endfor %}
    </div>
  </section>
</div>