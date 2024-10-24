---
layout: default
title: Philosophy
permalink: /philosophy/
---

<div class="philosophy-container">
    <h1>Philosophical Writings</h1>
    
    <div class="content-grid">
        {% for post in site.philosophy %}
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