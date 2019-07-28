---
layout: default
title: Blog
permalink: /blog/
---
<div class="container">
    <div class="blog-header">
        <h1>Latest</h1>
    </div>
    <div class="posts-container">
    {% for post in site.posts %}
        <div class="post-card">
            <div class="graphic">
                <a href="{{ post.url | prepend: site.baseurl }}">
                <img src="{{ post.cover-img }}"/>
                </a>
            </div>
            <div class="details">
                <h2><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
                <div class="meta">
                    <p class="date">
                        {% assign day = post.date | date: "%-d"  %}
                        {% case day %}
                            {% when '1' or '21' or '31' %}{{ day }}st
                            {% when '2' or '22' %}{{ day }}nd
                            {% when '3' or '23' %}{{ day }}rd
                        {% else %}{{ day }}th
                        {% endcase %}
                        {{ post.date | date: " %B %Y" }}
                    </p>
                    <div class="tags">{{ post.tags }}</div>
                </div>
                <div class="excerpt">{{ post.excerpt | strip_html | truncatewords:11 }}</div>
            </div>
        </div>        
    {% endfor %}
    </div>
</div>