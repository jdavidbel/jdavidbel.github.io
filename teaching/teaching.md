---
layout: page
permalink: /teaching/
title: Teaching
curs:
    - title:   "Engineering Math I Single Variable Calculus"
	  code:    "MATH1550:0134"
      year:    "Fall 2021"
      uni:     "The University of Iowa"
      url:     "/teaching/2020iieqdiff/" 
	- title:   "Mathematics for the Biological Sciences"
	  code:    "MATH1440:0A17"
	  year:    "Fall 2021"
	  uni:     "The University of Iowa"
	  url:     "/teaching/2020ii/1550/"
pasts:
    - title:   "Ecuaciones Diferenciales"
      <>note:  "In Spanish"
      year:    "2020-II"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     "/teaching/2020iiecdif/" 
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

## To the student: 
In this section I will include some readings and recommendations to improve how you learn and  how you can be more independent when learning.
- ¿Cómo escribir matemáticas? por Dr. Kevin P. Lee. [Texto](https://drive.google.com/file/d/16ZX_W6Cavz5x3HQockBGEuJxnasIT7LM/view?usp=sharing) 
- ¿Cómo enseñarse cosas? [Charla](https://drive.google.com/file/d/1scFYa1vfBog3Il0icdKs0MjSdB5pwipq/view?usp=sharing) 
<br> Esta charla es un resumen (muy corto) de las herramientas que hay disponibles para el aprendizaje autónomo. El énfasis en es aprender matemáticas y/o programación, pero estas herramientas sirven para todo.

- Tutoriales de Python [Videos y código](https://drive.google.com/drive/folders/1-cNsHTWosjvuEo8F7eOjHGevE88UzzoW?usp=sharing)

## Current
{% assign thumbnail="left" %}

{% for cur in page.curs %}
[**{{cur.title}}**]({% if cur.internal %}{{cur.url | prepend: site.baseurl}}{% else %}{{cur.url}}{% endif %})<br />
{{cur.uni}}<br />
*{{cur.year}}*
{% if cur.note %} *({{cur.note}})*
{% endif %}
{% endfor %}