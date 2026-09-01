---
title: Articles & Webpages
layout: page
permalink: /webpages
nav-include: true
nav-order: 2
---
## Articles

{% include big_three.md %}

{% for article in site.articles %}
<div>
<p>{{ article.content }}</p>
</div>
{% endfor %}


## General Resources

["Gender Equity Websites, Blogs, & Resources"](https://wcc.stanford.edu/community-resources-stanford/gender-equity-websites-blogs-resources) from Standford University

[Schlesinger Library History of Women in America Research Guides](https://guides.library.harvard.edu/schlesinger_rg_subject) from Harvard Library


## Blogs

[International Feminist Journal of Politics Blog](https://www.ifjpglobal.org/blog)  


<h2 id="books">Books</h2>
<small>PDFs of whole books.</small>  
    
{% for book in site.books %}
<div class="container">
<h4 class="book"><em><a href="/freefeminist-resources/{{ book.permalink }}">{{ book.title }}</a></em></h4> 
<small>by {{ book.author }}</small>
<p>{{ book.snip }}</p>
</div>
{% endfor %}