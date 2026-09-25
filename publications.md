---
layout: page
title: Publications
permalink: /publications/
kicker: Papers & chapters
lede: "† denotes a Smith College student co-author. Links go to the published version (DOI) where available."
---
{% if site.links.google_scholar != "" %}<p><a class="btn" href="{{ site.links.google_scholar }}">Google Scholar profile</a></p>{% endif %}

## Peer-reviewed articles and book chapters
{% assign by_year = site.data.publications | group_by: "year" %}
{% for y in by_year %}
<h3 class="year-h">{{ y.name }}</h3>
<ul class="pubs">{% for p in y.items %}{% include pub.html %}{% endfor %}</ul>
{% endfor %}

## In preparation
<ul class="pubs">{% for p in site.data.in_prep %}{% include pub.html %}{% endfor %}</ul>

## Other publications
<ul class="pubs">{% for p in site.data.other_pubs %}{% include pub.html %}{% endfor %}</ul>
