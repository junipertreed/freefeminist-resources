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

{% for post in site.documents %}
{% if post.type contains Book %}
<p><a href="/freefeminist-resources{{ post.url }}">{{ post.title }} by {{ post.author }}</a></p>
<p>{{ post.snip }}</p>
{% endif %}
{% endfor %}

{% for post in site.documents %}
{% if post.type contains Book %}
<a href="/freefeminist-resources{{ post.url }}">{{ post.title }}</a> {% if post.type %} {% unless post.type == blank %} | {{ post.type }} {% endunless %} {% endif %}
{% endif %}
{% endfor %}