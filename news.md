---
layout: page
title: News
permalink: /news/
---
<ul class="news">
{% for item in site.data.news %}
  <li><time datetime="{{ item.date | date_to_xmlschema }}">{{ item.date | date: "%b %Y" }}</time><p>{{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</p></li>
{% endfor %}
</ul>
