---
layout: sunny
permalink: /
title: "Home"
---

<section class="hero">
  <div class="hero-main">
    <img class="hero-avatar" src="{{ '/images/avatar.jpeg' | relative_url }}" alt="Tianya Zhao avatar">
    <div>
      <h1>Tianya Zhao (赵天涯)</h1>
      <p class="hero-sub">Ph.D. Candidate, Computer Science, Florida International University</p>
      <div class="hero-links">
        {% if site.author.googlescholar %}
        <a class="hero-link-chip" href="{{ site.author.googlescholar }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
        {% endif %}
        {% if site.author.email %}
        <a class="hero-link-chip" href="mailto:{{ site.author.email }}">Email</a>
        {% endif %}
        {% if site.author.linkedin %}
          {% if site.author.linkedin contains 'http' %}
        <a class="hero-link-chip" href="{{ site.author.linkedin }}" target="_blank" rel="noopener noreferrer">LinkedIn</a>
          {% else %}
        <a class="hero-link-chip" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" target="_blank" rel="noopener noreferrer">LinkedIn</a>
          {% endif %}
        {% endif %}
      </div>
    </div>
  </div>
  <p>My name is Tianya Zhao (赵天涯). I am a Ph.D. candidate studying computer science at Florida International University (FIU), supervised by <a href="https://users.cs.fiu.edu/~xuywang/">Dr. Xuyu Wang</a>. Prior to this, I received my Master’s degree from Carnegie Mellon University and my Bachelor’s degree from Hunan University.</p>
  <p>My research interest includes Trustworthy AI, AIoT, Wireless Sensing, LLMs for Time Series, and Smart Health. I am excited about the potential impact my research can have on the field of computer science and beyond. Outside of my academic pursuits, I like playing soccer⚽️ and hiking🧗.</p>
  <p class="job-tag">I am currently on the job market for faculty positions and industry research scientist roles.</p>
</section>

<section class="section-card" id="education">
  <h2>Education</h2>
  <ul>
    <li><strong>Expected June 2026</strong>: Ph.D. in Computer Science, Florida International University, Miami, FL, USA.</li>
    <li><strong>May 2022</strong>: M.Sc. in Civil and Environmental Engineering, Carnegie Mellon University, Pittsburgh, PA, USA.</li>
    <li><strong>June 2019</strong>: B.Eng. in Civil Engineering, Hunan University, Changsha, China.</li>
  </ul>
</section>

<section class="section-card" id="news">
  <h2>Latest News</h2>
  <!-- <p><strong>How to update:</strong> edit <code>_data/latest_news.yml</code> only. Add one new item at the top.</p> -->
  {% include latest-news.html limit=10 %}
</section>

<section class="section-card" id="teaching">
  <h2>Teaching</h2>
  <ul>
    <li><strong>Teaching Assistant</strong>, Machine Learning, Florida International University, Fall 2022 - Summer 2024.</li>
  </ul>
</section>

<section class="section-card">
  <h2>Visitor Map</h2>
  <div style="width: 220px; height: auto; overflow: hidden;">
    <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=Mlfw5u2_P8S719B3TKDw7wNb4-gZunfTvgXVLD0rLCY&cl=ffffff&w=a"></script>
  </div>
</section>
