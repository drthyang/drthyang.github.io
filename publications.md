---
layout: archive
title: "Publications"
author_profile: true
classes: wide
---

{% comment %} 
  Strict sorting: First we sort by year, then reverse it.
  If years are equal, Jekyll maintains the original order from the YAML file.
{% endcomment %}
{% assign pubs = site.data.publications | sort: 'year' | reverse %}

<style>
  .pub-list { 
    max-width: 1000px; 
    margin: 2rem auto; 
    color: #e0e0e0;
  }

  .pub-row { 
    margin-bottom: 1.5rem; /* Increased spacing for better scannability */
    display: flex; 
    gap: 30px; 
    border-bottom: 1px solid #333; 
    padding-bottom: 1.2rem;
  }
  
  .pub-year { 
    font-weight: 700; 
    color: #4facfe; /* Changed to accent color to anchor the timeline */
    font-size: 0.9rem; 
    min-width: 60px; 
    font-family: "Inter", -apple-system, sans-serif;
  }

  /* ... rest of your existing CSS ... */
  .pub-title { font-size: 1.05rem; font-weight: 700; color: #ffffff; margin-bottom: 6px; display: block; line-height: 1.3; }
  .pub-authors { font-size: 0.9rem; color: #b0b0b0; line-height: 1.3; margin-bottom: 6px; }
  .pub-venue { font-size: 0.9rem; font-style: italic; color: #999; }
  .me-bold { font-weight: 800; color: #ffffff; text-decoration: underline; text-decoration-color: #4facfe; text-underline-offset: 3px;}
  .link-bar { margin-top: 10px; font-size: 0.8rem; display: flex; gap: 15px; }
  .link-bar a { color: #4facfe; text-decoration: none; font-weight: 600; text-transform: uppercase; letter-spacing: 0.05em; }
  sub { font-size: 70%; line-height: 0; position: relative; vertical-align: baseline; bottom: -0.2em; color: #ffffff; }
</style>

<div class="pub-list">
{% for p in pubs %}
  <div class="pub-row">
    <div class="pub-year">{{ p.year }}</div>
    <div class="pub-content">
      <span class="pub-title">{{ p.title }}</span>
      <div class="pub-authors">
        {{ p.authors | replace: "T.-H. Yang", "<span class='me-bold'>T.-H. Yang</span>" | replace: "Tsung-Han Yang", "<span class='me-bold'>Tsung-Han Yang</span>" }}
      </div>
      <div class="pub-venue">{{ p.venue }}</div>
      <div class="link-bar">
        {% if p.links.doi != "" %}<a href="https://doi.org/{{ p.links.doi }}" target="_blank">DOI</a>{% endif %}
        {% if p.links.arxiv != "" %}<a href="https://arxiv.org/abs/{{ p.links.arxiv }}" target="_blank">ARXIV</a>{% endif %}
        {% if p.links.pdf != "" %}<a href="{{ p.links.pdf }}" target="_blank">PDF</a>{% endif %}
      </div>
    </div>
  </div>
{% endfor %}
</div>