---
layout: default
title: Projects
permalink: /projects/
---

<div class="projects-container">
    <h1 class="projects-title">Projects</h1>
    <p class="about-text" style="text-align: center; max-width: 600px; margin: 0 auto 40px auto; color: #666;">
        A collection of my work, ranging from data science experiments to web development projects.
    </p>

    <div class="projects-grid">
        {% for project in site.projects %}
            {% assign link_url = project.url %}
            {% assign is_external = false %}
            
            {% if project.external_url %}
                {% assign link_url = project.external_url %}
                {% assign is_external = true %}
            {% elsif project.github_repo %}
                {% assign link_url = project.github_repo %}
                {% assign is_external = true %}
            {% endif %}

            <a href="{{ link_url }}" class="project-card" {% if is_external %}target="_blank" rel="noopener noreferrer"{% endif %}>
                <div class="project-image-container">
                    {% if project.image %}
                        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
                    {% else %}
                        <!-- Fallback gradient if no image -->
                        <div class="gradient-overlay" style="width:100%; height:100%; background: linear-gradient(135deg, #fdfbfb 0%, #ebedee 100%);"></div>
                    {% endif %}
                </div>
                <div class="project-content">
                    <div class="project-type">
                        {% if project.github_repo %}
                            <i class="fa fa-github"></i> GitHub Project
                        {% elsif is_external %}
                            <i class="fa fa-link"></i> External Link
                        {% else %}
                            <i class="fa fa-file-text-o"></i> Case Study
                        {% endif %}
                    </div>
                    <h2 class="project-title">{{ project.title }}</h2>
                    <p class="project-description">
                        {% if project.description %}
                            {{ project.description | truncate: 120 }}
                        {% else %}
                            {{ project.content | strip_html | truncate: 120 }}
                        {% endif %}
                    </p>
                    <div class="project-footer">
                        <span class="project-link-text">
                            {% if is_external %}
                                View Project <i class="fa fa-external-link" style="margin-left: 5px; font-size: 0.8em;"></i>
                            {% else %}
                                Read More <i class="fa fa-arrow-right" style="margin-left: 5px; font-size: 0.8em;"></i>
                            {% endif %}
                        </span>
                    </div>
                </div>
            </a>
        {% endfor %}
    </div>
</div>
