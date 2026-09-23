---
title: Masoud Zarepisheh
description: Masoud Zarepisheh, Associate Professor/Attending in the Department of Medical Physics at Memorial Sloan Kettering Cancer Center. Mathematical optimization for radiotherapy treatment planning, the ECHO automated planning system, and the open-source PortPy project.
---

<div class="profile">
  <img class="profile-photo" src="{{ '/assets/masoud.png' | relative_url }}" alt="Masoud Zarepisheh">
  <div class="profile-text">
    <h1>Masoud Zarepisheh</h1>
    <p>Associate Professor/Attending<br>
    <a href="https://www.mskcc.org/departments/medical-physics">Department of Medical Physics</a><br>
    <a href="https://www.mskcc.org/">Memorial Sloan Kettering Cancer Center</a><br>
    321 East 61st Street, New York, NY 10065</p>
    <p class="profile-links">
      <a href="mailto:zarepism@mskcc.org">Email</a><span>·</span>
      <a href="https://scholar.google.com/citations?user=DuytjrMAAAAJ">Google Scholar</a><span>·</span>
      <a href="https://www.linkedin.com/in/masoud-zarepisheh-457a492b/">LinkedIn</a><span>·</span>
      <a href="https://github.com/masoudzp">GitHub</a>
    </p>
  </div>
</div>

<p class="lede">I develop mathematical optimization methods for radiotherapy treatment planning and translate them into clinical practice. Our automated planning system, <a href="#echo">ECHO</a>, is part of the daily clinical routine at Memorial Sloan Kettering, where it has been used to treat more than 12,000 patients, and it was a finalist for the 2021 INFORMS Franz Edelman Award. I also lead <a href="#portpy">PortPy</a>, an open-source Python platform that gives researchers benchmark data and algorithms for treatment planning optimization.</p>

## Research

<img class="banner" src="{{ '/assets/linac-msk.jpg' | relative_url }}" alt="A linear accelerator treatment room at Memorial Sloan Kettering">

Radiotherapy treats cancer with precisely directed radiation beams, and every patient's plan (beam angles, beam shapes, and intensities) must be tailored to that patient's anatomy and the physician's prescription for the tumor and the surrounding healthy tissue. Mathematically, this is a *large-scale*, *multi-criteria*, and often *non-convex* optimization problem, and my work is about solving it well enough, and fast enough, to be used in the clinic.

<h3 id="echo"><img class="inline-logo" src="{{ '/assets/edelman.jpg' | relative_url }}" alt="">Automated clinical planning: ECHO</h3>

Treatment planning has traditionally required hours of manual parameter tuning, with plan quality depending on the planner's skill and experience. ECHO (Expedited Constrained Hierarchical Optimization) automates this with hierarchical constrained optimization. It is integrated into the FDA-approved commercial treatment planning system [Eclipse](https://www.varian.com/products/radiotherapy/treatment-planning/eclipse), runs in our daily clinical routine, and has been used to treat more than 12,000 patients. ECHO was a finalist for the 2021 INFORMS Franz Edelman Award ([Video](https://www.youtube.com/watch?v=895M6j5KjPs&t=1025s) · [Slides]({{ '/assets/Edelman-ECHO-Slides.pdf' | relative_url }}) · [Paper](https://pubsonline.informs.org/doi/abs/10.1287/inte.2021.1095) · [Podcast](https://pubsonline.informs.org/do/10.1287/orms.2021.02.24p) · [Press](https://www.informs.org/About-INFORMS/News-Room/Press-Releases/Finalists-Selected-for-the-World-s-Leading-Operations-Research-and-Analytics-Award-2021-INFORMS-Franz-Edelman-Competition-Elevates-Research-that-is-Saving-Lives-Saving-Money-and-Solving-Problems)).

<h3 id="portpy"><img class="inline-logo" src="{{ '/assets/portpy-logotype.png' | relative_url }}" alt="">Open-source planning research: PortPy</h3>

[PortPy](https://github.com/PortPy-Project/PortPy) is an open-source Python package that provides research-ready *data* and *code* to speed up the development and clinical translation of treatment planning optimization algorithms. It ships benchmark data pre-calculated with Eclipse and benchmark implementations of beamlet, beam-angle, aperture, and robust optimization.

## Selected publications

<ul class="pubs">
{% for pub in site.data.publications %}{% if pub.selected %}{% include pub.html pub=pub show_tag=true %}{% endif %}{% endfor %}
</ul>

<p class="muted">Full list on the <a href="{{ '/CV/#publications' | relative_url }}">CV page</a> and on <a href="https://scholar.google.com/citations?user=DuytjrMAAAAJ">Google Scholar</a>.</p>
