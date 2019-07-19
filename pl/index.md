---
layout: default
title: Accueil
lang: pl
permalink: /pl
---

<div class="row">
  <div class="col-12 text-center">
    {% if site.gallery == false %}
      <p>Witajcie na naszej ślubnej stronie  !</p>
      <p>Zapraszamy Was bardzo serdecznie na nasz ślub kościelny,<br />
        który odbędzie się w <strong>sobotę 25 lipca 2020 o 15:00</strong>,<br />
      w kościele pw. Podwyższenia Krzyża Św. w <strong>Sławkowie</strong>.</p>
      <p>Przyjęcie odbędzie się w <strong>Lawendowym Dworku</strong> w Kluczach, przy ul.<br />Bolesławskiej 53A.</p>
      <div class="pt-2">
        <button type="button" class="btn btn-outline-danger">{{ site.data.translations.page.index.rsvp[page.lang] }}</button>
      </div>
     {% else %}
      <p>Merci à tous pour ce moment inoubliable !<br/>Voici quelques photos de cette magnifique journée...</p>
      {% include image-gallery.html folder="/uploads/album" %}
    {% endif %}   
  </div>
</div>
