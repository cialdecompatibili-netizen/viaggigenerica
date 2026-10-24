---
layout: single
title: "Viaggi di nozze"
permalink: /pacchetti/viaggi-di-nozze/
description: "Proposte romantiche costruite sui vostri tempi e sul vostro budget."
ref: cat-viaggi-di-nozze
classes: wide
author_profile: false
---
<p class="nv-lead">Proposte romantiche costruite sui vostri tempi e sul vostro budget.</p>

{% assign items = site.pacchetti | where: "cat", "viaggi-di-nozze" | where: "lang", page.lang | sort: "ordine" %}
{% if items.size > 0 %}<div class="nv-grid">
{% for t in items %}{% include pacchetto-card.html t=t %}{% endfor %}
</div>{% else %}<p class="nv-vuoto">Le proposte di questa categoria sono in preparazione. Scrivici cosa cerchi: ti prepariamo un preventivo su misura.</p>{% endif %}

<p class="nv-nota">Non trovi quello che cerchi? <a href="{% include url-ref.html ref="contatti" %}">Scrivici</a> o guarda i <a href="{% include url-ref.html ref="su-misura" %}">viaggi su misura</a>. <a href="{% include url-ref.html ref="pacchetti" %}">Tutti i viaggi</a>.</p>

