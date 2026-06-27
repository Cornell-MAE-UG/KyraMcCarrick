---
layout: default
title: Kyra McCarrick
---

## Hi, I'm Kyra McCarrick!


![Profile Picture]({{ "assets/images/KyraMcCarrickHeadshot.jpg" | relative_url }}){: class="profile-image"}


**I am a Senior pursuing a B.S. in Mechanical Engineering at Cornell University, and a [Division 1 varsity rower]({{ '/projects/2026-Rowing/' | relative_url }}).**

My academic foundation in mechanical engineering has equipped me with a rigorous, analytical approach to problem-solving.

I have translated those concepts into my internship, driving the engineering design process from initial ideation and CAD prototyping through to rigorous testing and refinement.

I am a motivator by action. I am committed to consistency, and prioritize the discipline required to perform regardless of circumstance whether in rowing or projects. People like working with me because I inspire a culture of resilience while keeping things upbeat and collaborative. I believe in the process, holding myself to a high standard, learning from each step, and seeing projects through with excellence.


<div style="display: flex; flex-wrap: wrap; justify-content: center; align-items: center; gap: 15px; background-color: #f8f9fa; padding: 16px 24px; border-radius: 8px; border: 1px solid #e9ecef; margin-top: 30px; margin-bottom: 30px;">
    
    <!-- Email Link -->
    <a href="mailto:kyramccarrick@gmail.com" style="text-decoration: none; color: #0056b3; font-weight: 600;">Email</a>
    
    <span style="color: #adb5bd;">&bull;</span>
    
    <!-- LinkedIn Link -->
    <a href="https://www.linkedin.com/in/kyra-mccarrick-1926351b5" target="_blank" style="text-decoration: none; color: #0056b3; font-weight: 600;">LinkedIn</a>
    
    <span style="color: #adb5bd;">&bull;</span>
    
    <!-- Projects Link -->
    <a href="#projects" style="text-decoration: none; color: #0056b3; font-weight: 600;">Projects</a>
    
    <span style="color: #adb5bd;">&bull;</span>
    
    <!-- Rowing Page Link -->
    <a href="{{ '/projects/2026-Rowing/' | relative_url }}" style="text-decoration: none; color: #0056b3; font-weight: 600;">Rowing</a>
    
    <span style="color: #adb5bd;">&bull;</span>
    
    <!-- Resume Request Link -->
    <a href="mailto:kyramccarrick@gmail.com?subject=Resume%20Request&body=Hi%20Kyra%2C%0D%0A%0D%0APlease%20send%20us%20a%20copy%20of%20your%20resume." style="text-decoration: none; color: #0056b3; font-weight: 600;">Resume</a>

</div>

<h2 id="projects" style="margin-top: 60px; margin-bottom: 30px; text-align: center;">My Projects</h2>

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
    <div class="gallery-item">
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
        <p>{{ project.title }}</p>
      </a>
    </div>
    {% endfor %}
  </div>
</div>
