---
layout: page
title: "Publications"
permalink: /publications/
---

<ul>
  {% assign pubs = site.data.publications | sort: "publication_year" | reverse %}
  {% for pub in pubs %}
    <li>
      <strong>{{ pub.title }}</strong><br>
      {% assign highlighted_authors = pub.authors | replace: "Bachanová, Petra", "<em><strong>Bachanová, Petra</strong></em>" %}
      <em>{{ highlighted_authors }}</em><br>
      {{ pub.journal }}, {{ pub.publication_year }}.
      {% if pub.url %}
        <a href="{{ pub.url }}" target="_blank">[Link]</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>