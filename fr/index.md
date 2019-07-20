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
        <button 
          role="button" 
          class="btn btn-danger btn-lg" 
          data-toggle="modal" 
          data-target=".bd-example-modal-xl">
            {{ site.data.translations.page.index.rsvp[page.lang] }}
        </button>
      </div>
      <div 
        class="modal fade bd-example-modal-xl" 
        tabindex="-1" 
        role="dialog" 
        aria-labelledby="rsvpForm" 
        aria-hidden="true">
        <div class="modal-dialog modal-xl">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="exampleModalLabel">{{ site.data.translations.page.index.rsvp[page.lang] }}</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfqMh-5hcBYwPeZ_0W--_GYqzMT47EIkpon4MZAE99A3Nj8gw/viewform?embedded=true" width="100%" height="1421" frameborder="0" marginheight="0" marginwidth="0">Chargement en cours...</iframe>
            </div>
          </div>
        </div>
      </div>
      <div id="introText">
        <p>Bienvenue sur le site de notre mariage !</p>
        <p>Nous sommes heureux de vous inviter à notre mariage religieux,<br />
          le <strong>samedi 25 juillet 2020 à 15 heures</strong>,<br />
        en l'église paroissiale de <strong>Sławków</strong> (Pologne).</p>
        <p>Veuillez nous rejoindre pour la fête<br />
        qui aura lieu à <strong>Lawendowy Dworek</strong>,<br />
        situé à Klucze, au 53 rue Bolesławska.</p>
      </div>
    {% else %}
      <p>Merci à tous pour ce moment inoubliable !<br/>Voici quelques photos de cette magnifique journée...</p>
      {% include image-gallery.html folder="/uploads/album" %}
    {% endif %}
  </div>
</div>