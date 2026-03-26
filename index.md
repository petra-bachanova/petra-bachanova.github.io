---
layout: home
permalink: /
---

<div class="profile-container">
  <!-- Left side: image and icons -->
  <div class="profile-left">
    <img src="/assets/img/me.png" alt="My picture" style="width: 100%; border-radius: 50%;">
    <div class="social-icons" style="margin-top: 1em; display: flex; justify-content: center; gap: 0.8em; color: #333;">
      {% if site.social.github %}
        <a href="{{ site.social.github }}" target="_blank" title="GitHub" style="color: inherit;">
          <i class="fab fa-github fa-lg"></i>
        </a>
      {% endif %}
      {% if site.social.orcid %}
        <a href="{{ site.social.orcid }}" target="_blank" title="ORCID" style="color: inherit;">
          <i class="fab fa-orcid fa-lg"></i>
        </a>
      {% endif %}
      {% if site.social.scholar %}
        <a href="{{ site.social.scholar }}" target="_blank" title="Google Scholar" style="color: inherit;">
          <i class="fas fa-graduation-cap fa-lg"></i>
        </a>
      {% endif %}
      {% if site.social.linkedin %}
        <a href="{{ site.social.linkedin }}" target="_blank" title="LinkedIn" style="color: inherit;">
          <i class="fab fa-linkedin fa-lg"></i>
        </a>
      {% endif %}
    </div>
  </div>

  <!-- Right side: intro text -->
  <div class="profile-right">
    <p style="font-size: 0.9em; line-height: 1.6;">
      Hello! I'm Petra. I'm a neuroscience PhD researcher, studying epilepsy genetics.<br><br>
      My research focuses on mutations that arise during brain development (rather than being inherited) and how they might increase the risk of epileptic seizures or influence clinical outcomes in patients. I study this by analysing EEG recordings and -omics data, using Python, R, and (reluctantly) MATLAB.<br><br>
      When I'm not in the lab, I try to spend as much time as possible outdoors or woodworking (see projects). <br><br>
      Welcome to my site!
    </p>
  </div>
</div>
