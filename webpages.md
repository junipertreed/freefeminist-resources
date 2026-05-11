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
<h4><a href="/freefeminist-resources/{{book.permalink}}">{{ book.title }} by {{ book.author }}</a></h4>
<p>{{ book.snip }}</p>
{% endfor %}