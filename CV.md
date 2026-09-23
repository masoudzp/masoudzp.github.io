---
title: CV
permalink: /CV/
description: Appointments, education, honors, and the full publication list of Masoud Zarepisheh.
---

# CV

<p class="jump"><a href="#appointments">Appointments</a><span>·</span><a href="#education">Education</a><span>·</span><a href="#honors">Honors</a><span>·</span><a href="#publications">Publications</a></p>

## Appointments

- **Associate Professor/Attending**, Department of Medical Physics, Memorial Sloan Kettering Cancer Center (2015–present)
- **Postdoctoral Fellow**, School of Medicine and Department of Management Science and Engineering, Stanford University (2013–2015). Supervisors: [Lei Xing](https://med.stanford.edu/xinglab.html), [Yinyu Ye](http://web.stanford.edu/~yyye/)
- **Postdoctoral Fellow**, Department of Radiation Medicine and Applied Sciences, University of California, San Diego (2011–2013). Supervisor: [Steve B. Jiang](https://sites.google.com/a/cart.ucsd.edu/main/people-1/directors/steve-b-jiang-ph-d)

## Education

- **Ph.D., Applied Mathematics (Operations Research)**, 2006–2011 · [Thesis]({{ '/assets/Thesis.pdf' | relative_url }})<br>
  Department of Industrial and Systems Engineering, University of Florida, and Department of Mathematics and Computer Science, Amirkabir University of Technology, Tehran, Iran. Supervisors: [Panos M. Pardalos](https://www.ise.ufl.edu/pardalos/), [Esmaile Khorram](https://aut.ac.ir/cv/2139/Esmaile%20Khorram)

## Honors

- **Franz Edelman Award finalist** (2021), Institute for Operations Research and the Management Sciences (INFORMS)
- **Clinical Service Award** (2019), Department of Medical Physics, Memorial Sloan Kettering Cancer Center
- **Norm Baily Best Paper Award** (2012), American Association of Physicists in Medicine (AAPM), Southern California Chapter
- **Ranked first** (2003), nationwide M.Sc. entrance exam in Applied Mathematics, Iran
- **Ranked third** (2003), nationwide M.Sc. entrance exam in Systems and Industrial Engineering, Iran

## Publications

<p class="muted">Also on <a href="https://scholar.google.com/citations?user=DuytjrMAAAAJ">Google Scholar</a>.</p>

{% assign years = site.data.publications | map: "year" | uniq %}
{% for y in years %}
<h3 class="cv-year" id="y{{ y }}">{{ y }}</h3>
<ul class="pubs">
{% for pub in site.data.publications %}{% if pub.year == y %}{% include pub.html pub=pub %}{% endif %}{% endfor %}
</ul>
{% endfor %}
