---
layout: single
title: "Vacanze in famiglia"
permalink: /pacchetti/famiglie/
description: "Soluzioni pensate per chi viaggia con bambini."
ref: cat-famiglie
classes: wide
author_profile: false
---
<p class="nv-lead">Soluzioni pensate per chi viaggia con bambini.</p>

{% assign items = site.pacchetti | where: "cat", "famiglie" | where: "lang", page.lang | sort: "ordine" %}
{% if items.size > 0 %}<div class="nv-grid">
{% for t in items %}{% include pacchetto-card.html t=t %}{% endfor %}
</div>{% else %}<p class="nv-vuoto">Le proposte di questa categoria sono in preparazione. Scrivici cosa cerchi: ti prepariamo un preventivo su misura.</p>{% endif %}

<p class="nv-nota">Non trovi quello che cerchi? <a href="{% include url-ref.html ref="contatti" %}">Scrivici</a> o guarda i <a href="{% include url-ref.html ref="su-misura" %}">viaggi su misura</a>. <a href="{% include url-ref.html ref="pacchetti" %}">Tutti i viaggi</a>.</p>

