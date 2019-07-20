---
layout: default
title: Accueil
lang: pl
permalink: /pl/
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
              <iframe src="https://docs.google.com/forms/d/e/1FAIpQLScs8RIJ4ZQ-uIVZ_xG_xuNndGWNyGh4Z1FCaGgw2BDL86A28A/viewform?embedded=true" width="100%" height="1421" frameborder="0" marginheight="0" marginwidth="0">Chargement en cours...</iframe>
            </div>
          </div>
        </div>
      </div>
      <div id="introText">
        <p>Witajcie na naszej ślubnej stronie  !</p>
        <p>Zapraszamy Was bardzo serdecznie na nasz ślub kościelny,<br />
          który odbędzie się w <strong>sobotę 25 lipca 2020 o 15:00</strong>,<br />
        w kościele pw. Podwyższenia Krzyża Św. w <strong>Sławkowie</strong>.</p>
        <p>Przyjęcie odbędzie się w <strong>Lawendowym Dworku</strong> w Kluczach, przy ul.<br />Bolesławskiej 53A.</p>
       {% else %}
        <p>Merci à tous pour ce moment inoubliable !<br/>Voici quelques photos de cette magnifique journée...</p>
        {% include image-gallery.html folder="/uploads/album" %}
      </div>
    {% endif %}   
  </div>
</div>
