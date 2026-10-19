---
layout: page
permalink: /publications/
title: Publications
description: Journal articles, manuscripts in preparation, and conference presentations, most recent first.
nav: true
nav_order: 1
---

<!-- _pages/publications.md
     Lists come from _bibliography/publications.bib and presentations.bib,
     the same files the LaTeX CV uses. Presentation lines are formatted by
     _includes/hook/bib.liquid. -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

## journal articles

<div class="publications">

{% bibliography --query @*[keywords!=preprint, keywords!=inprep] %}

</div>

{% capture inprep_count %}{% bibliography_count --query @*[keywords=inprep] %}{% endcapture %}
{% assign inprep_count = inprep_count | strip | plus: 0 %}
{% if inprep_count > 0 %}

## manuscripts in preparation

<div class="publications">

{% bibliography --query @*[keywords=inprep] %}

</div>

{% endif %}

{% capture preprint_count %}{% bibliography_count --query @*[keywords=preprint] %}{% endcapture %}
{% assign preprint_count = preprint_count | strip | plus: 0 %}
{% if preprint_count > 0 %}

## preprints

<div class="publications">

{% bibliography --query @*[keywords=preprint] %}

</div>

{% endif %}

## presentations

<div class="publications">

{% bibliography --file presentations %}

</div>

<p class="footnote-legend"><sup>*</sup> Corresponding author</p>
