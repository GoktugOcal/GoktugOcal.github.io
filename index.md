---
layout: default
title: "Home"
---

<div class="landing-container">
   <!-- Header Section: Photo Left, Name Right -->
   <div class="landing-header">
      <div class="landing-photo">
         <img class="img-pp" src="assets/img/pp3.webp" alt="Göktuğ Öcal">
      </div>
      <div class="landing-name">
         <h1 class="name-title">Göktuğ Öcal</h1>
         <p class="name-subtitle">Data Scientist & Computer Engineer</p>
         <div class="social-links">
            <a class="icon-link" rel="nofollow" href="https://www.linkedin.com/in/goktugocal" aria-label="LinkedIn"><i class="fa fa-linkedin fa-lg"></i></a>
            <a class="icon-link" rel="nofollow" href="https://github.com/GoktugOcal" aria-label="GitHub"><i class="fa fa-github fa-lg"></i></a>
            <a class="icon-link" rel="nofollow" href="https://medium.com/@goktugocal41" aria-label="Medium"><i class="fa fa-medium fa-lg"></i></a>
            <!-- <a class="icon-link" rel="nofollow" href="https://www.instagram.com/goktug.ocal/" aria-label="Instagram"><i class="fa fa-instagram fa-2x"></i></a> -->
            <a class="icon-link" rel="nofollow" href="https://open.spotify.com/user/mr41showtime?si=aa3902b9a7c74034" aria-label="Spotify"><i class="fa fa-spotify fa-lg"></i></a>
            <a class="icon-link" rel="nofollow" href="/assets/cv/Goktug_Ocal_CV.pdf" aria-label="CV"><i class="fa fa-file-pdf-o fa-lg"></i></a>
         </div>
      </div>
   </div>

   <!-- About Section -->
   <div class="landing-about">
      <p class="about-text">
         Hello!
      </p>
      <p class="about-text">
         I'm a Data Scientist currently exploring the intersection of industrial systems and intelligent algorithms at <strong>Daikin Europe N.V.</strong> My work focuses on leveraging data to drive innovation in sustainable climate solutions.
      </p>
      <p class="about-text">
         I hold an M.S. in Computer Engineering from <strong>Bogazici University</strong> and a B.S. in Control & Automation Engineering from <strong>Istanbul Technical University</strong>. I'm passionate about data science, F1, cinema, video games, and The Office.
      </p>
      <div class="landing-buttons">
         <a class="btn btn-minimal-mail" href="mailto:goktugocal41@gmail.com" role="button">Mail me</a>
         <a class="btn btn-minimal-cv" href="/assets/cv/Goktug_Ocal_CV.pdf" role="button" download="GoktugOcal_CV.pdf">Download my CV</a>
      </div>
   </div>

   <!-- Recent Writings Section -->
   <div class="landing-about" style="margin-top: 40px;">
      <h3 class="name-title" style="font-size: 1.1rem; margin-bottom: 20px;">Recent Writings</h3>
      <ul style="list-style-type: none; padding: 0; margin: 0;">
         {% for post in site.posts limit:3 %}
         <li style="margin-bottom: 15px;">
            <a href="{{ post.url }}" style="text-decoration: none; display: flex; align-items: flex-start; margin-bottom: 15px;">
               {% if post.cover %}
                  <img src="{{ post.cover }}" alt="{{ post.title }}" style="width: 48px; height: 48px; object-fit: cover; border-radius: 10%; margin-right: 15px; flex-shrink: 0;">
               {% else %}
                  <div style="width: 48px; height: 48px; background-color: #eee; border-radius: 10%; margin-right: 15px; flex-shrink: 0;"></div>
               {% endif %}
               <div>
                  <span class="about-text" style="display: block; margin-bottom: 4px; color: #2c2c2c; font-weight: 500; line-height: 1.4;">{{ post.title }}</span>
                  <span class="about-text" style="display: block; margin-bottom: 0; font-size: 0.85em; color: #999;">{{ post.date | date: "%d %b, %Y" }}</span>
               </div>
            </a>
         </li>
         {% endfor %}
      </ul>
   </div>

   <!-- Recent Projects Section -->
   <div class="landing-about" style="margin-top: 40px;">
      <h3 class="name-title" style="font-size: 1.1rem; margin-bottom: 20px;">Recent Projects</h3>
      <ul style="list-style-type: none; padding: 0; margin: 0;">
         {% for project in site.projects limit:3 %}
            {% assign link_url = project.url %}
            {% assign is_external = false %}
            
            {% if project.external_url %}
                {% assign link_url = project.external_url %}
                {% assign is_external = true %}
            {% elsif project.github_repo %}
                {% assign link_url = project.github_repo %}
                {% assign is_external = true %}
            {% endif %}

         <li style="margin-bottom: 15px;">
            <a href="{{ link_url }}" {% if is_external %}target="_blank" rel="noopener noreferrer"{% endif %} style="text-decoration: none; display: flex; align-items: flex-start; margin-bottom: 15px;">
               {% if project.image %}
                  <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" style="width: 48px; height: 48px; object-fit: cover; border-radius: 10%; margin-right: 15px; flex-shrink: 0;">
               {% else %}
                  <div style="width: 48px; height: 48px; background: linear-gradient(135deg, #fdfbfb 0%, #ebedee 100%); border-radius: 10%; margin-right: 15px; flex-shrink: 0;"></div>
               {% endif %}
               <div>
                  <span class="about-text" style="display: block; margin-bottom: 4px; color: #2c2c2c; font-weight: 500; line-height: 1.4;">{{ project.title }}</span>
                  <span class="about-text" style="display: block; margin-bottom: 0; font-size: 0.85em; color: #999;">
                      {% if project.github_repo %}GitHub Project{% elsif is_external %}External Link{% else %}Case Study{% endif %}
                  </span>
               </div>
            </a>
         </li>
         {% endfor %}
      </ul>
   </div>
</div>