---
layout: single
title: "Beach and holidays"
permalink: /en/packages/beach-and-holidays/
description: "Week-long beach holidays and resort stays, in Italy and abroad."
ref: cat-mare-vacanze
classes: wide
author_profile: false
lang: en
locale: en
tr: tradotto
tr_hash: 1hvx0e3
---
<p class="nv-lead">Week-long beach holidays and resort stays, in Italy and abroad.</p>

{% assign items = site.pacchetti | where: "cat", "mare-vacanze" | where: "lang", page.lang | sort: "ordine" %}
{% if items.size > 0 %}<div class="nv-grid">
{% for t in items %}{% include pacchetto-card.html t=t %}{% endfor %}
</div>{% else %}<p class="nv-vuoto">The proposals in this category are being prepared. Tell us what you are looking for: we will prepare a tailor-made quote.</p>{% endif %}

<p class="nv-nota">Cannot find what you are looking for? <a href="{% include url-ref.html ref="contatti" %}">Write to us</a> or see the <a href="{% include url-ref.html ref="su-misura" %}">tailor-made trips</a>. <a href="{% include url-ref.html ref="pacchetti" %}">All trips</a>.</p>

