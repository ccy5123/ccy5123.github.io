---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description: Full curriculum vitae and a one-page resume (PDF).
---

<!-- Both PDFs are built from cv/cv.tex and cv/resume.tex by .github/workflows/deploy.yml
     on every push, using the same _bibliography/*.bib files as the publications page. -->

<p>
  <a href="{{ '/assets/pdf/cv.pdf' | relative_url }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">
    <i class="fa-solid fa-file-pdf"></i> Full CV (PDF)
  </a>
  <a href="{{ '/assets/pdf/resume.pdf' | relative_url }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">
    <i class="fa-solid fa-file-lines"></i> One-page resume (PDF)
  </a>
</p>

<object data="{{ '/assets/pdf/cv.pdf' | relative_url }}" type="application/pdf" width="100%" style="height: 85vh; min-height: 600px;" aria-label="Full CV">
  <p>Your browser cannot display the PDF here. <a href="{{ '/assets/pdf/cv.pdf' | relative_url }}">Download the full CV</a> instead.</p>
</object>
