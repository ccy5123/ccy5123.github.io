---
layout: page
permalink: /publications/
title: Publications
description: Journal articles, preprints, and conference presentations, most recent first.
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

{% bibliography --query @*[keywords!=preprint] %}

</div>

## preprints

<div class="publications">

{% bibliography --query @*[keywords=preprint] %}

</div>

## presentations

<div class="publications">

{% bibliography --file presentations %}

</div>
