---
title: About Us
layout: default
nav_order: 9995
author_footer: false
authors: 
  - key: kaj
    role: "Temp"
  - key: fioh
    role: "Temp"
---

# About Us

<br>

{% if page.authors %}
{% for author_item in page.authors %}
{% assign author = site.data.authors[author_item.key] %}
{% if author %}
<div id="about_{{ author_item.key }}" style="padding-bottom:3rem;">
    <div style="display:flex !important; align-items:center; gap:1rem;">
        <img src="{{ author.avatar | relative_url }}" alt="{{ author.name }}" class="author-profile-pic">
        <p style="font-size:1.5rem; margin:0rem; ">{{ author.name }}</p>
    </div>
    <span class="about-bio">{{ author.bio }}</span>
    {% if author.links %}
    <div class="about-links" style="font-size: 1rem; margin-top: 0.5rem;">
    {% for link in author.links %}
        <a href="{{ link.url }}">
        {{ link.label }}
        </a>
        {% unless forloop.last %}
        <span style="color: #ccc;">|</span>
        {% endunless %}
    {% endfor %}
    </div>
    {% endif %}
</div>
{% endif %}
{% endfor %}
{% endif %}