---
title: Articles & Webpages
layout: page
permalink: /webpages
nav-include: true
nav-order: 2
---
## Articles

{% include pressbooks_theory.md %}  

{% include big_three.md %}

{% for article in site.articles %}
<div>
<p>{{ article.content }}</p>
</div>
{% endfor %}

## General Resources

["Gender Equity Websites, Blogs, & Resources"](https://wcc.stanford.edu/community-resources-stanford/gender-equity-websites-blogs-resources) from Standford University

## Blogs

[International Feminist Journal of Politics Blog](https://www.ifjpglobal.org/blog)  

## Books  
<small>PDFs of whole books.</small>  

{% for book in site.books %}
<div class="container">
<h3 class="hi up"><a href="/freefeminist-resources/{{book.permalink}}">{{ book.title }}</a></h3>
<div class="content-left">
<p>{{ book.snip }}</p>
</div>
{% if book.image %}
{% unless book.image == blank %}
<div class="img-right">
    <figure class="img-inner">
    <img src="{{ book.image }}" alt="{{ book.imgalt }}">
    </figure>
</div>
{% endunless %}
{% endif %}
</div>
{% endfor %}