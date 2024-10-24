---
layout: default
title: Mathematics
permalink: /math/
---

<div class="math-container">
    <h1>Mathematical Explorations</h1>
    
    <div class="content-grid">
        {% for post in site.math %}
            <div class="content-card">
                <h2>{{ post.title }}</h2>
                {% if post.description %}
                    <p>{{ post.description }}</p>
                {% endif %}
                <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
                <a href="{{ post.url | relative_url }}">Read more →</a>
            </div>
        {% endfor %}
    </div>
</div>