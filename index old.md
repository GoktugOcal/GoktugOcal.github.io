---
layout: default
title: "Home"
---

<div class="main-banner">
   <!-- <div class="row align-items-center" style="width: 50%;margin: 0 auto;height:100%;"> -->
   <div class="row col-md-6 col-sm-12 align-items-center" style="margin: 0 auto;height:100%;">
      <div class="col-xl-8 col-xs-12 order-xl-1 order-2">
         <p style="font-family: 'Caveat', cursive; font-size: calc(20px + 0.52vw); line-height: 1;">SUP EVERYONE! I'M</p>
         <p style="font-family: 'Bebas Neue', cursive; font-size: calc(100px + 2.6vw); line-height: 1;">GÖKTUĞ</p>
         <p style="font-family: 'Open Sans', sans-serif; font-size: calc(20px + 0.52vw); line-height: 1; color: rgb(255,153,0,1);">Istanbul based Data Scientist.</p>
         <p style="font-family: 'Open Sans', sans-serif; font-size: calc(13px + 0.35vw); line-height: 1.2;">I'm a data scientist from Istanbul, working at REENGEN. I love cinema, every branch of sports, video games and The Office.</p>
         <p style="font-family: 'Open Sans', sans-serif; font-size: calc(13px + 0.35vw); line-height: 1.2;">Contact with me.</p>
      </div>
      <div class="col-xl-4 col-xs-12 order-1">
         <img class="img-pp rounded-circle" src="assets/img/profile.jpg" alt="">
      </div>
   </div>
</div>

<div class="row col-12 justify-content-center">
   <div class="col-md-6 col-sm-12 .ml-auto" style="width:100%">
      <h1 class="section-title">Latest Posts</h1>
      <div class="col-12 postcards">
         {% for post in site.posts %}
         <div class="col-12 postcard-container">
            <div class="row col-12">
               <a href="{{ post.url }}">
                  <div class="row postcard-image">
                     <div class="col-md-4 col-sm-12 .ml-auto">
                        <img class="postcard-image-img" src="{{ post.cover }}" alt="There will be blood" width="100%">
                     </div>
                  </div>
                  <div class="row col-12">
                     <div class="col-md-4 gradient-overlay"></div>
                     <div class="col-md-8">
                        <h1 class="postcard-text-title">{{ post.title }}</h1>
                        <p class="postcard-text-summary">{{ post.summary }}</p>
                     </div>
                  </div>
               </a>
            </div>
         </div>
         {% endfor %}
      </div>
   </div>
</div>