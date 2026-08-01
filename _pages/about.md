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
      <p class="hero-sub">Senior Research Scientist, Origin AI<br>Ph.D. in Computer Science, Florida International University</p>
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
  <p>My name is Tianya Zhao (赵天涯). I am a Senior Research Scientist at Origin AI, where I continue to work on Wi-Fi sensing and AI applications. I received my Ph.D. in Computer Science from Florida International University (FIU), advised by <a href="https://users.cs.fiu.edu/~xuywang/">Dr. Xuyu Wang</a>. Prior to that, I received my Master’s degree from Carnegie Mellon University and my Bachelor’s degree from Hunan University.</p>
  <p>My research interests include Trustworthy AI, AIoT, Wireless Sensing, Wi-Fi Sensing, LLMs for Time Series, and Smart Health. I am particularly interested in building intelligent sensing systems that bridge wireless signals, machine learning, and real-world applications. Outside of my research, I enjoy playing soccer ⚽️ and hiking 🧗.</p>
</section>

<section class="section-card" id="education">
  <h2>Education</h2>
  <ul>
    <li><strong>July 2026</strong>: Ph.D. in Computer Science, Florida International University, Miami, FL, USA.</li>
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
