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
    <p>Tanya is an Assistant Professor of Genomics in the Department of Biological Sciences at Smith College. She earned her Ph.D. in Conservation Genomics from the University of Massachusetts Amherst, where her dissertation examined the conservation genomics of the threatened Canada lynx in the Northern Appalachian–Acadian ecoregion. She was then a Fulbright Scholar at the Estación Biológica de Doñana (CSIC) in Spain. As an NSF Postdoctoral Research Fellow in Biology, she worked with Elinor Karlsson at the Broad Institute of MIT and Harvard, Liliana Dávalos at Stony Brook University, and Emma Teeling at University College Dublin. She also received pedagogical training as an NIH IRACDA Fellow.</p>
    <p>Tanya leads the Bat1K Longevity Project, serves as Conservation Genomics Lead for the Vertebrate Genomes Project and as Bat1K representative to the Global Bat Network, and has served on the Federal Advisory Committee for Canada lynx since 2018. She is also Scientific Advisor in comparative genomics and molecular evolution at Paratus Sciences.</p>
    <p><a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a> · <a href="{{ '/cv/' | relative_url }}">Curriculum vitae</a></p>
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
{% assign featured_alumni = site.data.people.alumni | where_exp: "a", "a.photo" %}
<div class="people">{% for m in featured_alumni %}{% assign m = m %}{% include person.html %}{% endfor %}</div>
<ul class="alumni" style="margin-top:22px">
{% for a in site.data.people.alumni %}{% unless a.photo %}<li><strong>{{ a.name }}</strong><span>{{ a.now }}</span></li>{% endunless %}{% endfor %}
</ul>

<h3>Past undergraduate researchers</h3>
<p class="namecloud">{{ site.data.people.past_undergraduates | join: " · " }}</p>
