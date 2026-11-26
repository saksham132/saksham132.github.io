---
layout: page
title: Off the Bench
---
Things I do when I’m not in the lab. Each week I post a new photo and, when I can, a song I’ve been learning.

## Photo of the week {#photos}

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

## Guitar of the week {#guitar}

I’m learning guitar and posting a short video of a new song each week.

{% assign songs = site.songs | sort: "date" | reverse %}
{% if songs.size > 0 %}
{% for s in songs %}
<div class="song"><span class="d">{{ s.date | date: "%b %-d, %Y" }}</span><span><a href="{{ s.youtube }}">{{ s.title }}</a>{% if s.artist %} <span class="muted">· {{ s.artist }}</span>{% endif %}{% if s.note %}<br><span class="muted">{{ s.note }}</span>{% endif %}</span></div>
{% endfor %}
{% else %}
<p class="empty">The first song is coming soon.</p>
{% endif %}
