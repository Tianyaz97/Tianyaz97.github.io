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
  <div class="news-slider-wrap" data-news-slider>
    <button class="news-nav news-nav-prev" aria-label="Previous news" data-news-prev>&larr;</button>
    <div class="news-slider" data-news-track>
      <article class="news-card"><p class="news-date">Feb 2026</p><p>One paper accepted by IEEE/CVF CVPR 2026. Congratulations, Jingzhou.</p></article>
      <article class="news-card"><p class="news-date">Jan 2026</p><p><em>EMPalm</em> accepted by ACM SenSys 2026. Congratulations, Haowen.</p></article>
      <article class="news-card"><p class="news-date">Oct 2025</p><p>One paper accepted by IEEE TMC.</p></article>
      <article class="news-card"><p class="news-date">Oct 2025</p><p>Invited to serve as TPC member of IEEE ICNC 2026.</p></article>
      <article class="news-card"><p class="news-date">Mar 2025</p><p>Passed dissertation proposal defense.</p></article>
      <article class="news-card"><p class="news-date">Feb 2025</p><p>One paper accepted by ACM SenSys 2025.</p></article>
    </div>
    <button class="news-nav news-nav-next" aria-label="Next news" data-news-next>&rarr;</button>
  </div>
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

<script>
  document.addEventListener('DOMContentLoaded', function () {
    var root = document.querySelector('[data-news-slider]');
    if (!root) return;
    var track = root.querySelector('[data-news-track]');
    var prev = root.querySelector('[data-news-prev]');
    var next = root.querySelector('[data-news-next]');

    function step() {
      return Math.max(280, Math.round(track.clientWidth * 0.72));
    }

    prev.addEventListener('click', function () {
      track.scrollBy({ left: -step(), behavior: 'smooth' });
    });

    next.addEventListener('click', function () {
      track.scrollBy({ left: step(), behavior: 'smooth' });
    });
  });
</script>
