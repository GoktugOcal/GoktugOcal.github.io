---
layout: default
title: Projects
permalink: /projects/
---

<div class="blog">
    <div class="section-header">
         <h1 class="section-title title">Projects</h1>
         <p class="section-subtitle text" style="margin-bottom: 40px;">A marked list of my projects, experiments and open-source contributions.</p>
    </div>
    <div class="col-12">
        {% assign sorted_projects = site.projects | sort: "path" %}
        {% for project in sorted_projects %}
            {% assign link_url = project.url %}
            {% assign is_external = false %}
            
            {% if project.external_url %}
                {% assign link_url = project.external_url %}
                {% assign is_external = true %}
            {% elsif project.github_repo %}
                {% assign link_url = project.github_repo %}
                {% assign is_external = true %}
            {% endif %}

             <div class="col-12 postcard-container">
                <a href="{{ link_url }}" title="{{ project.title }}" {% if is_external %}target="_blank" rel="noopener noreferrer"{% endif %}>
                    <div class="row">
                        <div class="col-12">
                             <h1 class="postcard-text-title title">
                                {{ project.title }}
                                {% if project.github_repo %} <i class="fa fa-github" style="font-size: 0.6em; vertical-align: middle; margin-left: 5px; color: #555;"></i>{% endif %}
                                {% if project.external_url %} <i class="fa fa-external-link" style="font-size: 0.6em; vertical-align: middle; margin-left: 5px; color: #555;"></i>{% endif %}
                             </h1>
                             <p class="postcard-text-summary text">
                                {% if project.description %}
                                    {{ project.description }}
                                {% else %}
                                    {{ project.content | strip_html | truncate: 150 }}
                                {% endif %}
                             </p>
                        </div>
                    </div>
                </a>
                
                <div class="col-12 date" style="padding:0px; display: flex; align-items: center; gap: 8px; flex-wrap: wrap; margin-top: 10px;">
                    <span style="font-family: 'Oswald', sans-serif; font-size: 0.8rem; color: #666; margin-bottom: 0;">
                        {% if project.date %}
                            {{ project.date | date: "%d %b %Y" }}
                        {% endif %}
                    </span>
                    {% if project.tags %}
                    <span style="color: #444;">•</span>
                    <span class="tags" style="font-family: 'Oswald', sans-serif; font-size: 0.8rem; color: #666; margin-bottom: 0;">
                         {% for tag in project.tags %}
                             {{ tag }}{% unless forloop.last %}, {% endunless %}
                         {% endfor %}
                    </span>
                    {% endif %}
                </div>
             </div>
        {% endfor %}
    </div>
</div>
