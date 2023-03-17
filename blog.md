---
layout: default
title: "Personal Blog"
---


<div class="blog row col-12 justify-content-center" style="margin: 0px;">
   <div class="col-lg-6 col-md-10 col-sm-12" style="padding: 0px;">
      <h1 class="section-title">All Posts</h1>
      <div class="col-12">
         {% for post in site.posts %}
         {% assign read_time = post.content | number_of_words | divided_by: 200 %}
         <div class="col-12 postcard-container">
            <a href="{{ post.url }}"  title="{{ post.title }}">
                <div class="row">
                    <div class="col-md-4 col-sm-12 postcard-image">
                        {% if post.cover %}
                            <img class="postcard-image-img" src="{{ post.cover }}" width="100%">
                            <!--https://raw.githubusercontent.com/GoktugOcal/GoktugOcal.github.io/master-->
                        {% else %}
                            <img class="postcard-image-img" style="background-color: var(--white-2);" width="100%">
                        {% endif %}
                    </div>
                    <div class="col-md-8 col-sm-12">
                        <h1 class="postcard-text-title">{{ post.title }}</h1>
                        <div class="col-12 date-info" style="padding:0px;">
                            {% if post.updated %}
                                <p>Updated at {{ post.updated | date: "%d %b %Y" }}</p>
                                <p> | Created at {{ post.date | date: "%d %b %Y" }}</p>
                            {% else %}
                                <p>{{ post.date | date: "%d %b %Y" }} | {{read_time}} min read</p>
                            {% endif %}
                        </div>
                        <p class="postcard-text-summary">{{ post.summary }}</p>
                        <div class="tags">
                            {% for tag in post.tags %}
                                <div class="tag" style="background-color: {{ site.data.tag_colors[0][tag] }};" href="/blog/{{ tag }}">{{ tag }}</div>
                            {% endfor %}
                        </div>
                    </div>
                </div>
            </a>
         </div>
         {% endfor %}
      </div>
   </div>
</div>