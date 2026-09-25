---
layout: page
title: People
permalink: /people/
kicker: The lab
---
<div class="pi">
  <img src="{{ '/assets/img/people/tanya-lama.jpg' | relative_url }}" alt="Portrait of Dr. Tanya M. Lama" width="600" height="600">
  <div>
    <h2 style="margin-top:0">Tanya M. Lama, PhD</h2>
    <p class="kicker" style="margin-bottom:14px">Principal Investigator · Assistant Professor of Genomics</p>
    <p>Dr. Tanya Lama received her doctorate from UMass Amherst and completed the National Science Foundation Postdoctoral Research Fellowship in Biology jointly hosted by the Dávalos Lab at SUNY Stony Brook and the Karlsson Lab at the Broad Institute of MIT & Harvard. Using genomic methods, Dr. Lama studies the evolutionary processes underlying population vulnerability, resilience, and response, particularly in the context of global climate change. Her applied conservation research on Canada lynx <em>(L. canadensis)</em> demonstrates how genomics can bridge the gap between research, management, and policy. The Wildlife Genomics Lab at Smith College focuses on how life history traits -- particularly lifespan -- can shape evolutionary responses to rapid environmental change. Along with key collaborators <a href="https://lmdavalos.github.io/">Drs. Liliana Davalos (SUNY Stony Brook)</a> and <a href="http://batlab.ucd.ie/">Emma Teeling (University College Dublin)</a>, Dr. Lama uses comparative genomics to explore the evolution and mechanisms of aging in long-lived and short-lived species of bats and other mammals. In addition to her role as a research fellow, she received teaching pedagogy and leadership training from <a href="https://www.stonybrook.edu/commcms/iracda/">National Institutes of Health NY-CAPS IRACDA </a> – a targeted program for the development of underrepresented minority scholars in biomedical research.</p>
    <p><a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a> · <a href="{{ site.links.faculty_profile }}">Smith faculty profile</a> · <a href="{{ site.links.google_scholar }}">Google Scholar</a> · <a href="{{ '/cv/' | relative_url }}">CV highlights</a></p>
  </div>
</div>

{% if site.data.people.faculty.size > 0 %}
## Faculty & research scientists
<div class="people">{% for m in site.data.people.faculty %}{% include person.html %}{% endfor %}</div>
{% endif %}

## Graduate students
<div class="people">{% for m in site.data.people.graduate %}{% include person.html %}{% endfor %}</div>

## Undergraduate researchers
<div class="people">{% for m in site.data.people.undergraduate %}{% if m.photo or m.bio %}{% include person.html %}{% endif %}{% endfor %}</div>
<ul class="alumni" style="margin-top:22px">
{% for m in site.data.people.undergraduate %}{% unless m.photo or m.bio %}<li><strong>{{ m.name }}</strong><span>{{ m.role }}</span></li>{% endunless %}{% endfor %}
</ul>

## Lab alumni

### Where are they now?
<div class="people">{% for m in site.data.people.where_now %}{% include person.html hide_initials=true %}{% endfor %}</div>

### Former lab members
<ul class="alumni" style="margin-top:12px">
{% for a in site.data.people.alumni %}<li><strong>{{ a.name }}</strong><span>{{ a.now }}</span></li>{% endfor %}
</ul>

<h3>Past undergraduate researchers</h3>
<p class="namecloud">{{ site.data.people.past_undergraduates | join: " · " }}</p>
