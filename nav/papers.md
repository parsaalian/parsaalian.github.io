---
layout: default
title: Papers
permalink: /papers/
weight: 3
group: pubs
---



{% assign papers_by_year = site.data.papers | group_by_exp:"paper", "paper.year | plus: 0" %}
{% for year in papers_by_year %}
  <h3>{{ year.name }}</h3>
  {% for paper in year.items %}
  <div class="publication" id="{{ paper.id }}">
    {% if paper.award %}
    <span class="icon">
      <svg><use xlink:href="#icon-award"/></svg>
      <b>{{ paper.award }}</b>
    </span> <br/>
    {% endif %}
    <div class="publication-title">
      <b>
        <a href="{{ paper.url }}" target="_blank">{{ paper.title }}</a>
      </b>
      <br/>
      {{ paper.authors }}
      <br/>
      {% if paper.venue %}<i>{{ paper.venue }}</i>,{% endif %} {% if paper.pages %}{{ paper.pages }} pages,{% endif %} {{ paper.year }}.
    </div>
    <div class="right">
      {% if paper.id %}
      <a href="{{ "/resources/papers/" | append: paper.id | append: ".pdf" | prepend: site.baseurl }}" target="_blank">
        <span class="icon"><svg><use xlink:href="#icon-pdf"/></svg></span>
      </a>
      {% endif %}
      {% if paper.code %}
      <a href="{{ paper.code }}" target="_blank">
        <span class="icon"><svg><use xlink:href="#icon-github"/></svg></span>
      </a>
      {% endif %}
      {% if paper.video %}
      <a href="{{ paper.video }}" target="_blank">
        <span class="icon"><svg><use xlink:href="#icon-youtube"/></svg></span>
      </a>
      {% endif %}
    </div>
  </div>
  {% endfor %}
{% endfor %}
