---
layout: default_analytics
title: "analytics.go"
---


<div class="blog row col-12 justify-content-center" style="margin: 0px;">
   <div class="col-lg-6 col-md-10 col-sm-12" style="padding: 0px;">
      <h1 class="section-title">Analytics.</h1>
      <div class="col-12">
         {% for post in site.tools %}
         {% assign read_time = post.content | number_of_words | divided_by: 200 %}
         <div class="col-12 tools-card-container">
            <a href="{{ post.tool_url }}"  title="{{ post.title }}">
                <div class="row">
                    <div class="tools-card-image col-3 col-md-2">
                        {% if post.cover %}
                            <img class="tools-card-image-img" src="{{ post.cover }}">
                        {% else %}
                            <img class="postcard-image-img" style="background-color: var(--white-2);" width="100%">
                        {% endif %}
                    </div>
                    <div class="col-9 col-md-8 postcard-content">
                        <h1 class="postcard-text-title">{{ post.title }}</h1>
                        <p class="postcard-text-summary">{{ post.summary }}</p>
                    </div>
                    <div class="tool-tags col-md-2 col-0">
                        {% for tag in post.tags %}
                            <div class="tag" style="background-color: {{ site.data.tag_colors[0][tag] }};" href="/blog/{{ tag }}">{{ tag }}</div>
                        {% endfor %}
                    </div>
                </div>
            </a>
         </div>
         {% endfor %}
      </div>
   </div>
</div>