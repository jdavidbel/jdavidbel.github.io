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

## Teaching responsabilities: 
I am a teaching assistant in the courses listed below. I'm responsible to lead discussion sections that are intented to complement
the weekly lectures that students attend in their respective courses. During the discussion sections important concepts of the courses are reviewed,
students work in groups to discuss and solve problems related to the topics of their courses and they have the opportunity to ask for clarifications and
ask for guidance to complete their assignments. 


## Current 
{% for past in page.pasts %}
[**{{past.title}}**]({% if past.internal %}{{past.url | prepend: site.baseurl}}{% else %}{{past.url}}{% endif %})<br />
{{past.uni}}<br />
*{{past.year}}*
{% if past.note %} *({{past.note}})*
{% endif %}
{% endfor %}


