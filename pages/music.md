---
layout: default
title: Music
permalink: /music/
---

<div class="music-container">
    <h1>Musical Explorations</h1>
    
    <div class="content-grid">
        {% for post in site.music %}
            <div class="content-card">
                <h2>{{ post.title }}</h2>
                {% if post.description %}
                    <p>{{ post.description }}</p>
                {% endif %}
                {% if post.embed_player %}
                    <div class="music-player">
                        {{ post.embed_player }}
                    </div>
                {% endif %}
                <a href="{{ post.url | relative_url }}">Read more →</a>
            </div>
        {% endfor %}
    </div>
</div>