---
layout: default
title: Fotografie
lang: pl
---

<div class="row">
  {% if site.gallery == false %}
    <div class="col-12 text-left">
      <p>Kilka dni po ślubie (będzie to zależało m.in. od naszego fotografa), będziecie mogli tu znaleźć galerię zdjęć z najważniejszych momentów naszego wyjątkowego dnia!</p>
    </div>
    <div class="col-12 text-center">
      {% include image-gallery.html folder="/uploads/waiting" %}
    </div>
  {% else %}
    <div class="col-12 text-center">
      <p>Dziękujemy wszystkim za te wspaniałe chwile!<br/>Oto kilka zdjęć zrobionych tego cudownego dnia...</p>
      {% include image-gallery.html folder="/uploads/album" %}
    </div>
  {% endif %}
</div>