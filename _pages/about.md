---
layout: archive
author_profile: false
title: About
permalink: /about/
---

Hi,

I am Michal Franc and this is my site.

## About me

{{ site.author.bio }}

## Where to go next

{% if site.author.links %}
    {% for link in site.author.links %}
        {% if link.label and link.url %}
<ul class="author__urls social-icons">
    <li>
        <a href="{{ link.url }}" rel="nofollow noopener noreferrer">
            <i class="{{ link.icon | default: 'fas fa-link' }}" aria-hidden="true"></i>
            <span class="label">{{ link.label }}</span>
        </a>
    </li>
</ul>
        {% endif %}
    {% endfor %}
{% endif %}