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
          {% if pub.url %}
            <a href="{{ pub.url }}" target="_blank">{{ pub.title }}.</a>
          {% else %}
            {{ pub.title }}.
          {% endif %}
        </strong>
        <span>
          {% assign authors = pub.authors | split: "," %}
          {% for author in authors %}
            {% assign author = author | strip %}
            {% if author contains "Petra" %}
              <u>{{ author }}</u>{% unless forloop.last %},{% endunless %}
            {% else %}
              {{ author }}{% unless forloop.last %},{% endunless %}
            {% endif %}
          {% endfor %}
        </span>, <em>{{ pub.journal }}</em>, {{ pub.publication_year }}.
      </span>
    </li>
  {% endfor %}
</ul>
