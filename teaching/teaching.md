---
layout: page
permalink: /teaching/
title: Teaching
curs:
    - title:   "Ecuaciones Diferenciales"
      <>note:  "In Spanish"
      year:    "2020-II"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     "/teaching/ecdif2020ii/" 
pasts:
    - title:   "Ecuaciones Diferenciales"
      <>note:  "In Spanish"
      year:    "2020-I"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     https://sites.google.com/unal.edu.co/ecdif-2020i/
    - title:   "Química I"
      <>note:  ""
      year:    "2017-I to 2019-I"
      uni:     "Universidad Central"
      url:
    - title:   "Fisicoquímica I"
      <>note:  ""
      year:    "2017-I"
      uni:     "Universidad Central"
      url:
---

## Current
{% assign thumbnail="left" %}

{% for cur in page.curs %}
[**{{cur.title}}**]({% if cur.internal %}{{cur.url | prepend: site.baseurl}}{% else %}{{cur.url}}{% endif %})<br />
{{cur.uni}}<br />
*{{cur.year}}*
{% if cur.note %} *({{cur.note}})*
{% endif %}
{% endfor %}

## Past 
{% for past in page.pasts %}
[**{{past.title}}**]({% if past.internal %}{{past.url | prepend: site.baseurl}}{% else %}{{past.url}}{% endif %})<br />
{{past.uni}}<br />
*{{past.year}}*
{% if past.note %} *({{past.note}})*
{% endif %}
{% endfor %}
