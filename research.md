---
layout: page
title: Research
---
## Current research

I’m in the Shendure Lab, working on improving paired prime editing: how efficiently we can insert sequences into the genome, and how to enrich the cells that carry the edit. I’m also interested in RNA biology and in using genome editing to ask functional questions at scale.

*(Placeholder. Edit this paragraph to describe your work the way you would.)*

## Publications

<div class="pub">
Rominger MC, O’Brien S, Gupta S, Moorthi S, McSharry M, Kamlapurkar S, Lowe AR, Waldum A, Lo A, Duke F, Wu F, Headley MB, Cromwell E, Glabman R, Koehne A, Berger AH. Mutant RIT1 cooperates with YAP to drive an EMT-like lung cancer state. (2025) PMID: 41004338
<div class="links"><a href="https://pubmed.ncbi.nlm.nih.gov/41004338/">PubMed</a><a href="https://doi.org/10.1016/j.celrep.2025.116185">Cell Reports</a><a href="https://doi.org/10.1101/2024.11.11.623044">bioRxiv</a></div>
</div>

## Summaries {#summaries}

A short summary of one paper I read each week.

{% assign papers = site.papers | sort: "date" | reverse %}
{% if papers.size > 0 %}
<ul class="recent">
{% for p in papers %}
  <li><span class="d">{{ p.date | date: "%b %-d, %Y" }}</span><span><a href="{{ p.url | relative_url }}">{{ p.title }}</a>{% if p.journal %} <span class="muted">· {{ p.journal }}</span>{% endif %}</span></li>
{% endfor %}
</ul>
{% else %}
<p class="empty">The first summary is coming soon.</p>
{% endif %}
