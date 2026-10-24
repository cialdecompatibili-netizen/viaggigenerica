---
layout: single
title: "Family holidays"
permalink: /en/packages/family-holidays/
description: "Solutions designed for those travelling with children."
ref: cat-famiglie
classes: wide
author_profile: false
lang: en
locale: en
tr: tradotto
tr_hash: 1ewsw4z
---
<p class="nv-lead">Solutions designed for those travelling with children.</p>

{% assign items = site.pacchetti | where: "cat", "famiglie" | where: "lang", page.lang | sort: "ordine" %}
{% if items.size > 0 %}<div class="nv-grid">
{% for t in items %}{% include pacchetto-card.html t=t %}{% endfor %}
</div>{% else %}<p class="nv-vuoto">The proposals in this category are being prepared. Tell us what you are looking for: we will prepare a tailor-made quote.</p>{% endif %}

<p class="nv-nota">Cannot find what you are looking for? <a href="{% include url-ref.html ref="contatti" %}">Write to us</a> or see the <a href="{% include url-ref.html ref="su-misura" %}">tailor-made trips</a>. <a href="{% include url-ref.html ref="pacchetti" %}">All trips</a>.</p>

