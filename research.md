---
layout: page
title: Research
---
I’m interested in functional and computational genomics: how we can write to the genome precisely, and how to read out what those changes do. In my PhD I work on improving prime editing, and I’m also interested in RNA biology. Earlier I studied how oncogenic RIT1 reshapes lung cancer cells, and used single-cell multiomics to look for early markers of tumorigenesis.

<p><a href="{{ '/assets/files/Saksham_Gupta_CV.pdf' | relative_url }}">Download my CV (PDF)</a></p>

## Publications

<div class="pub">
Rominger MC, O’Brien S, Gupta S, Moorthi S, McSharry M, Kamlapurkar S, Lowe AR, Waldum A, Lo A, Duke F, Wu F, Headley MB, Cromwell E, Glabman R, Koehne A, Berger AH. Mutant RIT1 cooperates with YAP to drive an EMT-like lung cancer state. (2025) PMID: 41004338
<div class="links"><a href="https://pubmed.ncbi.nlm.nih.gov/41004338/">PubMed</a><a href="https://doi.org/10.1016/j.celrep.2025.116185">Cell Reports</a><a href="https://doi.org/10.1101/2024.11.11.623044">bioRxiv</a></div>
</div>

## Talks and posters

- Gupta S, Rominger C, Moorthi S, Berger A. Single-cell profiling of RIT1-mutant tumor model reveals an EMT phenotype. Post-baccalaureate Scholar Symposium, Fred Hutch (June 2024)
- Gupta S. Single-cell phenotyping of RIT1-driven lung cancer. Cancer GeVo Seminar Series, Fred Hutch (July 2024)
- O’Brien S, Gupta S, Waldum A, Berger A. Dissecting paralog transcriptional adaptation through functional genomics. Human Biology Retreat, Fred Hutch (September 2023)

## Research experience

**Graduate research assistant** · University of Washington, Genome Sciences · Apr 2025 – present  
Advisor: Jay Shendure. Improving paired prime editing efficiency and enrichment: screening a library of insertion designs for features linked to higher editing rates, and testing fluorescence-based strategies to enrich edited cells by FACS.

**Rotation student** · Fred Hutch Cancer Center, Setty Lab · Sep – Dec 2025  
Analyzed paired scATAC-seq and scRNA-seq from matched tumor and normal head and neck cancer samples, and found a “tumor-primed” epithelial subpopulation in normal tissue whose chromatin accessibility changes preceded gene expression changes.

**Post-baccalaureate scholar** · Fred Hutch Cancer Center, Berger Lab · Jul 2023 – Apr 2025  
Characterized a RIT1-driven lung cancer mouse model with single-cell RNA-seq, showing that lung epithelial cells move to an EMT-like state, and standardized CUT&RUN to study RIT1–YAP transcription factor binding.

**Summer intern** · Fred Hutch Cancer Center, Berger Lab · May – Jul 2022  
Built direct-capture Perturb-seq libraries and validated genetic compensation between the paralogs CCNL1 and CCNL2.

**Undergraduate researcher** · IIT Kanpur, Zafar Lab · Dec 2021 – Dec 2022  
Benchmarked how hyperparameters affect clustering of single-cell RNA-seq data.

## Papers I’ve read {#reading}

A short summary of one paper each week.

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
