---
layout: single
title: "Tour organizzati"
permalink: /pacchetti/tour-organizzati/
description: "Circuiti con itinerario già pronto, in Italia e nel mondo."
ref: cat-tour-organizzati
classes: wide
author_profile: false
---
<p class="nv-lead">Circuiti con itinerario già pronto, in Italia e nel mondo.</p>

{% assign items = site.pacchetti | where: "cat", "tour-organizzati" | where: "lang", page.lang | sort: "ordine" %}
{% if items.size > 0 %}<div class="nv-grid">
{% for t in items %}{% include pacchetto-card.html t=t %}{% endfor %}
</div>{% else %}<p class="nv-vuoto">Le proposte di questa categoria sono in preparazione. Scrivici cosa cerchi: ti prepariamo un preventivo su misura.</p>{% endif %}

<p class="nv-nota">Non trovi quello che cerchi? <a href="{% include url-ref.html ref="contatti" %}">Scrivici</a> o guarda i <a href="{% include url-ref.html ref="su-misura" %}">viaggi su misura</a>. <a href="{% include url-ref.html ref="pacchetti" %}">Tutti i viaggi</a>.</p>

