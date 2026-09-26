---
layout: page
title: Curriculum Vitae
permalink: /cv/
kicker: Tanya M. Lama, PhD
---
{% assign cvfile = site.static_files | where: "path", site.cv_pdf | first %}
<p class="btns" style="margin-top:0">{% if cvfile %}<a class="btn primary" href="{{ site.cv_pdf | relative_url }}">Download full CV (PDF)</a>{% endif %}<a class="btn{% unless cvfile %} primary{% endunless %}" href="{{ site.links.faculty_profile }}">Smith faculty profile</a><a class="btn" href="{{ site.links.google_scholar }}">Google Scholar</a></p>

## Appointments

- **Assistant Professor of Genomics**, Department of Biological Sciences, Smith College (2023–present)
- **NSF Postdoctoral Research Fellow in Biology**, Broad Institute of MIT and Harvard, with Stony Brook University and University College Dublin (2021–2023)
- **NIH IRACDA Fellow**, Stony Brook University (2021–2022)
- **Fulbright Scholar**, Estación Biológica de Doñana, CSIC, Spain (2020–2021)

## Education

- **Ph.D. Conservation Genomics**, University of Massachusetts Amherst (2021). *Conservation genomics of the threatened Canada lynx (Lynx canadensis) in the Northern Appalachian–Acadian ecoregion*
- **M.S. Molecular Ecology**, University of Massachusetts Amherst (2017). *Stress response in African elephants and analysis of their post-release movements*
- **B.S. Biology**, University of Connecticut (2013)

## Selected funding

- Blakeslee Fund Endowment, Smith College (2024, 2025)
- American Federation for Aging Research TIME Fellowship, to M. Weber (2024)
- Horner Fund Endowment Summer Fellowship, to A. Batista (2024)
- NSF Postdoctoral Research Fellowship in Biology (2020)
- UMass Amherst Natural History Collections (2018)
- U.S. Fish & Wildlife Service, Canada Lynx Status Investigation (2017)

See [Publications]({{ '/publications/' | relative_url }}), [Teaching]({{ '/teaching/' | relative_url }}), and [Outreach]({{ '/outreach/' | relative_url }}) for more.
