---
layout: page
title: Off the Bench
---
<p class="jump"><a href="#teaching">Teaching and service</a> · <a href="#photography">Photography</a> · <a href="#guitar">Guitar</a> · <a href="#misc">Miscellaneous</a></p>

## Teaching and service {#teaching}

I care about widening who gets to do science, especially for students from communities that are underrepresented in it.

- **Sunday Science, Seattle Public Library (May 2026).** A public science outreach event.
- **Genome Sciences Retreat, University of Washington (Sept 2026).** Helped organize the department retreat.
- **Rural teaching, IIT Kanpur (2019 – 2020).** Through the National Service Scheme I coordinated an effort to enroll students in the Navodaya teaching program in nearby villages, with a focus on girls in STEM. I helped design a curriculum and taught weekly math and science classes to about 60 students.
- **Openscapes Champions Program, Fred Hutch (2023).** Workshops on open, reproducible data science. I used these practices to run lab inventory and day-to-day tasks with GitHub issues.

## Photography {#photography}

I’m trying to get into photography. A new photo each week.

{% assign photos = site.photos | sort: "date" | reverse %}
{% if photos.size > 0 %}
<div class="gallery">
{% for p in photos %}
  <figure>
    <img src="{{ p.image | relative_url }}" alt="{{ p.alt | default: p.title }}" loading="lazy">
    <figcaption><b>{{ p.title }}</b>{% if p.place %} · {{ p.place }}{% endif %}<br>{{ p.date | date: "%b %-d, %Y" }}</figcaption>
  </figure>
{% endfor %}
</div>
{% else %}
<p class="empty">The first photo is coming soon.</p>
{% endif %}

## Guitar {#guitar}

I’m learning guitar and posting a short video of a new song each week.

{% assign songs = site.songs | sort: "date" | reverse %}
{% if songs.size > 0 %}
{% for s in songs %}
<div class="song"><span class="d">{{ s.date | date: "%b %-d, %Y" }}</span><span><a href="{{ s.youtube }}">{{ s.title }}</a>{% if s.artist %} <span class="muted">· {{ s.artist }}</span>{% endif %}{% if s.note %}<br><span class="muted">{{ s.note }}</span>{% endif %}</span></div>
{% endfor %}
{% else %}
<p class="empty">The first song is coming soon.</p>
{% endif %}

## Miscellaneous {#misc}

Puzzles and other odds and ends.

<p class="empty">Coming soon.</p>
