---
layout: home
permalink: /
---


<div style="display: flex; align-items: center; gap: 2em; max-width: 1000px; margin: auto;">
  <!-- Left side: image and icons -->
  <div style="flex: 2;">
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
  <div style="flex: 3; min-width: 300px;">
    <p style="font-size: 0.9em; line-height: 1.6;">
        Hi, I'm Petra - a neuro(data)science PhD student.<br><br>
        In my research I explore how the brain’s micro-world (cells, genes, proteins) gives rise to its macro-world (brain rhythms), to better understand neurological conditions such as epilepsy. I’m curious whether subtle differences in the structure and organization of brain cells - and their electrical activity - might help explain why some treatments in epilepsy work for certain individuals but not others.<br><br>
        To figure that out, I analyse complex medical data (EEG & omics) using Python, R, bash, and sometimes MATLAB (reluctantly).<br>
        I run a lot of things on HPC.<br><br>
        This site is just a little nook for my projects and research.<br>
        Welcome!
      <!-- Add your intro here -->
    </p>
  </div>
</div>

