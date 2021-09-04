---
layout: page
permalink: /teaching/
title: Teaching
---
{% assign thumbnail="left" %}

{% for cur in page.curs %} [{{cur.title}}]({% if cur.internal %}{{cur.url | prepend: site.baseurl}}{% else %}{{cur.url}}{% endif %})
{{cur.uni}}
{{cur.year}} {% if cur.note %} ({{cur.note}}) {% endif %} {% endfor %}