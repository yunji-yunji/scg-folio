---
layout: page
title: People
permalink: /people/
description: People of SCG
---

<div>
    <ul>
        {% for people in site.people %}
            <li>
                <a href="{{ people.url | prepend: site.baseurl | prepend: site.url }}">{{ people.profile.name }}</a>
            </li>
        {% endfor %}
    </ul>
</div>