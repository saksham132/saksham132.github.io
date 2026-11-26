---
layout: default
title: About
---
<div class="intro">
  <img src="{{ '/assets/img/saksham.jpg' | relative_url }}" alt="Saksham Gupta">
  <div>
    <h1>Saksham Gupta</h1>
    <p class="tagline">PhD student · Genome Sciences · University of Washington</p>
    <p>I’m a PhD student in the Shendure Lab at the University of Washington in Seattle. I work on genome editing and RNA biology, mixing wet-lab molecular biology (CRISPR, prime editing, RNA aptamers) with computational work on sequencing data. I started in the lab in April 2025 and joined the Genome Sciences program that September.</p>
  </div>
</div>

I did my undergraduate degree in mechanical engineering at IIT Kanpur, where an interest in cells and genomics pulled me toward biology. After that I spent two years as a post-baccalaureate scholar in Alice Berger’s lab at the Fred Hutch Cancer Center, studying RIT1-driven lung cancer with single-cell and epigenomic methods. That is where I learned to do both the experiments and the analysis, and I’ve wanted to do both ever since.

Away from the bench, I’m learning guitar, taking photographs, and trying to be a better teacher and mentor. See [Off the Bench]({{ '/off-the-bench/' | relative_url }}) and [Non-research]({{ '/non-research/' | relative_url }}).

## Recent

{% assign feed = site.papers | concat: site.songs | concat: site.photos | sort: "date" | reverse %}
{% if feed.size > 0 %}
<ul class="recent">
{% for item in feed limit: 6 %}
  <li><span class="d">{{ item.date | date: "%b %-d, %Y" }}</span>
  <span>
  {% if item.collection == "papers" %}<span class="tag">Paper</span><a href="{{ item.url | relative_url }}">{{ item.title }}</a>
  {% elsif item.collection == "songs" %}<span class="tag">Guitar</span><a href="{{ item.youtube }}">{{ item.title }}</a>
  {% else %}<span class="tag">Photo</span><a href="{{ '/off-the-bench/#photos' | relative_url }}">{{ item.title }}</a>{% endif %}
  </span></li>
{% endfor %}
</ul>
{% else %}
<p class="empty">Weekly paper summaries, photos and songs will show up here.</p>
{% endif %}
