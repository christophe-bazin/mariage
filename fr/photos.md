---
layout: default
title: Galerie
lang: fr
---

<div class="row">
  {% if site.gallery == false %}
    <div class="col-12 text-left">
      <p>Quelques heures ou quelques jours après le mariage (le temps pour nous de nous reposer), vous pourrez trouver ici une sélection des meilleurs moments de cette journée !</p>
    </div>
    <div class="col-12 text-center">
      {% include image-gallery.html folder="/uploads/waiting" %}
    </div>
  {% else %}
    <div class="col-12 text-center">
      <p>Merci à tous pour ce moment inoubliable !<br/>Voici quelques photos de cette magnifique journée...</p>
      {% include image-gallery.html folder="/uploads/album" %}
    </div>
  {% endif %}
</div>