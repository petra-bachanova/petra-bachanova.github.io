---
layout: page
title: "Publications"
permalink: /publications/
---

<ul>
  {% assign pubs = site.data.publications | sort: "publication_year" | reverse %}
  {% assign current_year = nil %}

  {% for pub in pubs %}
    {% if pub.publication_year != current_year %}
      {% assign current_year = pub.publication_year %}
      <h3>{{ current_year }}</h3>
    {% endif %}
    
    <li>
      <span>
        <strong>
          <a href="{{ pub.url }}" target="_blank">{{ pub.title }}</a>
        </strong>
        <span>
          <em>
            {{ pub.authors | replace: "[X], Petra", "<u>[X], Petra</u>" }}
          </em>
        </span>,
        <em>{{ pub.journal }}</em>, {{ pub.publication_year }}.
      </span>
    </li><br>
  {% endfor %}
</ul>
