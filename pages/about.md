---
layout: default
title: About
permalink: /about/
---

<div class="about-container">
    <div class="about-header">
        <img src="/assets/images/profile.jpg" alt="Profile Picture" class="about-image">
        <h1>About Me</h1>
    </div>

    <div class="about-content">
        <p>
            I'm interested in the science of research agents and inference-time scaling and work as a scientist at Google Research. I was born and raised in the Chicago metro, where I got my undergrad degree in mathematics and computer science from the University of Chicago. In my spare time I love writing, playing, and listening to Classical music, reading, and studying history and philosophy.
        </p>

        <section class="social-links-section">
            <h2>Links</h2>
            <ul class="social-list">
                <li><a href="https://x.com/{{ site.twitter_username }}">Twitter/X</a></li>
                <li><a href="https://github.com/{{ site.github_username }}">GitHub</a></li>
                {% if site.linkedin_url %}<li><a href="{{ site.linkedin_url }}">LinkedIn</a></li>{% endif %}
                {% if site.flatio_url %}<li><a href="{{ site.flatio_url }}">Flat.io</a></li>{% endif %}
            </ul>
        </section>
    </div>
</div>
