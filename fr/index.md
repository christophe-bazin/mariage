---
layout: default
title: Accueil
lang: fr
permalink: /fr/
---

<div class="row">
  <div class="col-12 text-center">
    {% if site.gallery == false %}
      <div class="pb-4">
        <a role="button" class="btn btn-danger btn-lg" href="formulaire-de-reponse">
          {{ site.data.translations.page.index.rsvp[page.lang] }}</a>
      </div>
      <p>Bienvenue sur le site de notre mariage !</p>
      <p>Nous sommes heureux de vous inviter à notre mariage religieux,<br />
        le <strong>samedi 25 juillet 2020 à 15 heures</strong>,<br />
      en l'église paroissiale de <strong>Sławków</strong> (Pologne).</p>
      <p>Veuillez nous rejoindre pour la fête<br />
      qui aura lieu à <strong>Lawendowy Dworek</strong>,<br />
      situé à Klucze, au 53 rue Bolesławska.</p>
    {% else %}
      <p>Merci à tous pour ce moment inoubliable !<br/>Voici quelques photos de cette magnifique journée...</p>
      {% include image-gallery.html folder="/uploads/album" %}
    {% endif %}
  </div>
</div>