---
layout: single
title: "Publications"
author_profile: true
toc: true
toc_label: "Jump to Year"
toc_icon: "list"
toc_sticky: true
---

{% comment %} 
  Sorts strictly by year (newest first). 
  Items within the same year follow the order in your YAML file.
{% endcomment %}
{% assign pubs = site.data.publications | sort: "year" | reverse %}

<style>
  /* Container adjustment to fill the empty side space slightly better */
  .pub-list { 
    max-width: 1000px; 
    margin: 2rem auto; 
    color: #e0e0e0; /* Light grey primary text for dark mode */
  }

  .pub-row { 
    margin-bottom: 0rem; 
    display: flex; 
    gap: 30px; 
    border-bottom: 1px solid #333; /* Subtle divider for dark theme */
    padding-bottom: 0.5rem;
  }
  
  /* Muted grey for the year so it doesn't distract from titles */
  .pub-year { 
    font-weight: 700; 
    color: #888; 
    font-size: 0.8rem; 
    min-width: 60px; 
    font-family: "Inter", -apple-system, sans-serif;
  }

  /* Off-white for high readability on dark backgrounds */
  .pub-title { 
    font-size: 1.0rem; 
    font-weight: 700; 
    color: #ffffff; 
    margin-bottom: 6px; 
    display: block; 
    line-height: 1.3;
  }
  
  /* Slightly dimmer grey for authors */
  .pub-authors { 
    font-size: 0.9rem; 
    color: #b0b0b0; 
    line-height: 1.3; 
    margin-bottom: 6px; 
  }
  
  /* Italicized venue in a secondary color */
  .pub-venue { 
    font-size: 0.9rem; 
    font-style: italic; 
    color: #999; 
  }

  /* Highlighting your name: white and bold to stand out */
  .me-bold { 
    font-weight: 800; 
    color: #ffffff; 
    /* text-decoration: underline; 
    /* text-decoration-color: #4facfe; /* Subtle blue underline accent */
    text-underline-offset: 3px;
  }

  /* Link bar with a tech-friendly blue or gold accent */
  .link-bar { 
    margin-top: 10px; 
    font-size: 0.8rem; 
    display: flex;
    gap: 15px;
  }
  
  .link-bar a { 
    color: #4facfe; /* "Electric" blue that looks great on black/dark grey */
    text-decoration: none; 
    font-weight: 600; 
    text-transform: uppercase;
    letter-spacing: 0.05em;
    transition: color 0.2s ease;
  }
  
  .link-bar a:hover { 
    color: #00f2fe; /* Brighter glow on hover */
    text-decoration: underline;
  }

sub {
  font-size: 70%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
  bottom: -0.2em;
  color: #ffffff; /* Optional: Make the subscripts match your accent color */
}
</style>

<div class="pub-list">
{% for p in pubs %}
  <div class="pub-row">
    <div class="pub-year">{{ p.year }}</div>
    <div class="pub-content">
      <span class="pub-title">{{ p.title }}</span>
      <div class="pub-authors">
        {% comment %} Using replace for both possible formats of your name {% endcomment %}
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