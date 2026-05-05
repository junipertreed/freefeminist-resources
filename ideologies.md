---
title: Political and Philosophical Perspectives
layout: page
permalink: /ideologies
nav-include: true
---

There are various branches of feminism, all with different grounding philosophies. In the last 100 years, the three most influential have been liberal feminism, Marxist feminism, and radical feminism. 

## Feminist Ideologies

{% for ideology in site.ideologies %}
<div class="container">
<h3 class="hi up"><a href="/freefeminist-resources/{{ideology.permalink}}">{{ ideology.title }}</a></h3>
<div class="content-left">
<p>{{ ideology.snip }}</p>
</div>
{% if ideology.image %}
{% unless ideology.image == blank %}
<div class="img-right">
    <figure class="img-inner">
    <img src="{{ ideology.image }}" alt="{{ ideology.imgalt }}">
    <figcaption><a href="{{ ideology.imgsource }}">{{ ideology.imgcaption }}</a></figcaption>
    </figure>
</div>
{% endunless %}
{% endif %}
</div>
{% endfor %}
