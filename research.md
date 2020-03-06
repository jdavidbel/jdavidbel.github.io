---
layout: page
permalink: /research/
title: Research
books:
    - title:   "Process Analysis and Simulation in Chemical Engineering"
      author:  "Gil Chaves, I.D., López, J.R.G., García Zapata, J.L., Leguizamón Robayo, A., Rodríguez Niño, G."
      journal: "Springer International Publishing"
      <>note:  "(presented at Oz)"
      year:    "2016"
      image:   "https://images.springer.com/sgw/books/medium/9783319148113.jpg"
      url:     "https://www.springer.com/gp/book/9783319148113"
      doi:     "http://dx.doi.org/10.1007/978-3-319-14812-0"
    - title:   "Análisis y Simulación de Procesos en Ingeniería Química"
      author:  "Gil Chaves, I.D., López, J.R.G., García Zapata, J.L., Leguizamón Robayo, A."
      journal: "Editorial UN"
      <>note:  "Coleción 150 años Facultad de Ingeniería"
      year:    "2011"
      image:   "https://libu.s3.amazonaws.com/imgThumbnail/1881_9789587199109_unal-thmb.jpg"
      url:     "https://www.uneditorial.com/analisis-y-simulacion-de-procesos-en-ingenieria-quimica-ingenieria-en-general-1.htmlhttps://www.springer.com/gp/book/9783319148113"
      <>doi:     "http://dx.doi.org/10.1007/978-3-319-14812-0"
pubs:
    - title:   "Control of an azeotropic distillation process to acetonitrile production"
      author:  "Ruiz, A., Borda, N., Leguizamón, A., Guevara, J. R., Gil C., I.D."
      journal: "Computer Aided Chemical Engineering"
      note:    "Volume 29, Pages 833-838"
      year:    "2011"
      url:     "https://www.sciencedirect.com/science/article/pii/B978044453711950167X?via%3Dihub"
      doi:     "https://doi.org/10.1016/B978-0-444-53711-9.50167-X"
      <>media:
      <> - name: "IMDB"
      <>    url:  "http://www.imdb.com/title/tt0133093/"

---

## Publications
{% assign thumbnail="left" %}

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />URL: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}
## Books 

{% assign thumbnail="left" %}

{% for book in page.books %}
{% if book.image %}
{% include image.html url=book.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{book.title}}**]({% if book.internal %}{{book.url | prepend: site.baseurl}}{% else %}{{book.url}}{% endif %})<br />
{{book.author}}<br />
*{{book.journal}}*
{% if book.note %} *({{book.note}})*
{% endif %} *{{book.year}}* {% if book.doi %}[[doi]({{book.doi}})]{% endif %}
{% if book.media %}<br />URL: {% for article in book.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}
