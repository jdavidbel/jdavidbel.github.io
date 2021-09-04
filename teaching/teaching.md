---
layout: page
permalink: /teaching/
title: Teaching
curs:
    - title:   "Engineering Math I Single Variable Calculus"
      <>note:  "In English"
      year:    "Fall 2021"
      uni:     "The University of Iowa"
      url:     https://myui.uiowa.edu/my-ui/courses/details.page?ci=155573&id=941316
pasts:
    - title:   "Engineering Math I Single Variable Calculus"
      <>note:  "In English"
      year:    "Fall 2021"
      uni:     "The University of Iowa"
      url:     https://myui.uiowa.edu/my-ui/courses/details.page?ci=155573&id=941316 
    - title:   "Mathematics for the Biological Sciences"
      <>note:  "In English"
      year:    "Fall 2021"
      uni:     "The University of Iowa"
      url:     https://myui.uiowa.edu/my-ui/courses/details.page?ci=149667&id=941277
---

## To the student: 
In this section I will include some readings and recommendations to improve how you learn and  how you can be more independent when learning.
- ¿Cómo escribir matemáticas? por Dr. Kevin P. Lee. [Texto](https://drive.google.com/file/d/16ZX_W6Cavz5x3HQockBGEuJxnasIT7LM/view?usp=sharing) 
- ¿Cómo enseñarse cosas? [Charla](https://drive.google.com/file/d/1scFYa1vfBog3Il0icdKs0MjSdB5pwipq/view?usp=sharing) 
<br> Esta charla es un resumen (muy corto) de las herramientas que hay disponibles para el aprendizaje autónomo. El énfasis en es aprender matemáticas y/o programación, pero estas herramientas sirven para todo.

- Tutoriales de Python [Videos y código](https://drive.google.com/drive/folders/1-cNsHTWosjvuEo8F7eOjHGevE88UzzoW?usp=sharing)


## Current 
{% for past in page.pasts %}
[**{{past.title}}**]({% if past.internal %}{{past.url | prepend: site.baseurl}}{% else %}{{past.url}}{% endif %})<br />
{{past.uni}}<br />
*{{past.year}}*
{% if past.note %} *({{past.note}})*
{% endif %}
{% endfor %}


