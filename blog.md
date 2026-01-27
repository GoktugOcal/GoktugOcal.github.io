---
layout: default
title: "Personal Blog"
---


<div class="blog">
   <!-- <div class="col-lg-6 col-md-10 col-sm-12" style="padding: 0px;"> -->
       <div class="section-header">
         <h1 class="section-title title">Writings</h1>
         <p class="section-subtitle text" style="margin-bottom: 40px;">A personal blog where I share my thoughts, experiences, and technical insights.</p>
      </div>
      <div class="col-12">
         {% for post in site.posts %}
         {% assign read_time = post.content | number_of_words | divided_by: 200 %}
         <div class="col-12 postcard-container">
            <a href="{{ post.url }}"  title="{{ post.title }}">
                <div class="row">
                    <!-- <div class="col-md-4 col-sm-12 postcard-image">
                        {% if post.cover %}
                            <img class="postcard-image-img" src="{{ post.cover }}" width="100%">
                        {% else %}
                            <img class="postcard-image-img" style="background-color: var(--white-2);" width="100%">
                        {% endif %}
                    </div> -->
                    <div class="col-12">
                        <h1 class="postcard-text-title title">{{ post.title }}</h1>
                        <p class="postcard-text-summary text">{{ post.summary }}</p>
                    </div>
                </div>
            </a>
            <div class="col-12 date" style="padding:0px; display: flex; align-items: center; gap: 8px; flex-wrap: wrap; margin-top: 10px;">
                            <span style="font-family: 'Oswald', sans-serif; font-size: 0.8rem; color: #666; margin-bottom: 0;">
                                {% if post.updated %}
                                    Updated: {{ post.updated | date: "%d %b %Y" }}
                                {% else %}
                                    {{ post.date | date: "%d %b %Y" }}
                                {% endif %}
                            </span>
                            <span style="color: #444;">•</span>
                            <span class="tags" style="font-family: 'Oswald', sans-serif; font-size: 0.8rem; color: #666; margin-bottom: 0;">
                                {% for tag in post.tags %}
                                    {{ tag }}{% unless forloop.last %}, {% endunless %}
                                {% endfor %}
                            </span>
                        </div>
         </div>
         {% endfor %}
      </div>
   <!-- </div> -->
</div>