---
layout: default
title: Home
---
<div class="hero">
    <img src="/assets/images/profile.jpg" alt="Profile Picture">
    <h1>Welcome to my blog</h1>
    <p>A space for thoughts on work, math, philosophy, and music.</p>
</div>
<div class="recent-posts">
    <h2>Recent Posts</h2>
    <ul>
    {% for post in site.posts limit:5 %}
        <li>
            <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
            <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
            {% if post.description %}
                <p>{{ post.description }}</p>
            {% endif %}
        </li>
    {% endfor %}
    </ul>
</div>
