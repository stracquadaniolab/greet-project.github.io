---
title: Selected publications
layout: default
---
## Preprints
<OL>
{% for paper in site.data.publications %}
  {% if paper.ENTRYTYPE == 'preprint' %}
<li><a href="https://doi.org/{{ paper.doi }}" name="{{paper.ID}}">{{ paper.title }}</a>.  
{{ paper.author | replace: '*', '<sup>1</sup>'| replace: '^', '<sup>3</sup>'| replace: 'Stracquadanio', '<b>Stracquadanio</b>' }}, {{ paper.journal }}, {{ paper.year }}.</li>
  {% endif %}
{% endfor %}
</ol>
