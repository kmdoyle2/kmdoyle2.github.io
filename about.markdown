---
layout: single
title: About
permalink: /about/
classes: wide

team:
  - name: "Keegan Doyle"
    image_path: /assets/images/headshot1.jpg
    bio: "I am an Honors Computer Science student at The University of Alabama, currently pursuing a B.S. in Computer Science alongside an MBA through the STEM Path to the MBA program. With a background in both technical development and IT strategy, I have experience as a Web Development Intern at Kinetic Communications, where I managed front-end development and sitewide updates. Most recently, I served as an IT Analyst Intern at Milwaukee Tool, applying ITIL best practices and conducting User Acceptance Testing (UAT) to ensure system reliability. I am passionate about applying critical thinking to solve complex technical problems and delivering robust digital solutions."
  
  - name: "Tyler Bish"
    image_path: /assets/images/PlaceholderHeadshot.jpg
    bio: "[Enter Description Here]"

  - name: "Ayush Singh"
    image_path: /assets/images/PlaceholderHeadshot.jpg
    bio: "[Enter Description Here]"

  - name: "EJ Jones"
    image_path: /assets/images/PlaceholderHeadshot.jpg
    bio: "[Enter Description Here]"
---

## Meet the Team

<div class="team-container">
  {% for member in page.team %}
    <div class="team-member" style="display: flex; gap: 20px; margin-bottom: 40px; align-items: flex-start;">
      
      <div class="member-image" style="flex: 0 0 150px;">
        <img src="{{ member.image_path | relative_url }}" alt="{{ member.name }}" style="border-radius: 50%; width: 100%; height: auto; object-fit: cover;">
      </div>

      <div class="member-info">
        <h3 style="margin-top: 0;">{{ member.name }}</h3>
        {% if member.role %}
          <p style="font-weight: bold; color: #666;">{{ member.role }}</p>
        {% endif %}
        <p>{{ member.bio }}</p>
      </div>

    </div>
  {% endfor %}
</div>