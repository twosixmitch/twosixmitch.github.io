---
layout: default
title: Blog - Mitchell Duncan
permalink: /blog
category: blog
---
<div class="container blog">
  {% include blog-header.html %}
  <section class="section latest-posts">
    <h2>Latest posts</h2>
    <div class="posts-container">
      {% for post in site.posts %}
        {% include postcard.html %}        
      {% endfor %}
    </div>
  </section>
</div>