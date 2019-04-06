---
layout: page
title: Projects
permalink: /projects/
description: Our projects
---

{% for project in site.projects %}

<div class="project ">
    <div class="box" style="box-shadow: 0 3px 5px 0 rgba(0,1,1,.1);">
        <div class="thumbnail">
            <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
            {% if project.img %}
            <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
            {% else %}
            <div class="thumbnail blankbox"></div>
            {% endif %}    
            </a>
        </div>
        <div class="description" style="padding: 23px 30px 30px;">
            <div class="title" style="color: #111; font-size: 22px; font-weight: 700;">
                {{ project.title }}
            </div>
            <span>
                {{ project.description }}
            </span>
        </div>
    </div>
</div>

{% endfor %}
