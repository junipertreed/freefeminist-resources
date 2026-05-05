---
title: Basic Feminist Concepts
layout: page
permalink: /basics
nav-include: true
---

Simplified term defintions and background information, plus some introductional resources. 

## Feminist Vocabulary

These terms are used across different feminist theories. The nuances of the terms will change, but the basic meaning as presented here will stay the same.  


<div>
    {% for vocab in site.vocab %}
    {% if vocab.category contains "foundations" %}
    <div class="container">
    <h3><a href="/freefeminist-resources{{ vocab.permalink }}">{{ vocab.title }}</a></h3>
    <p>{{ vocab.content }}</p>
    </div>
    {% endif %}
    {% endfor %}
</div>


## Questions  

### What is feminist theory?  
{% include pressbooks_theory.md %}  

### Why do people separate Black feminism from feminism by race?  
Read "[The Revolutionary Practice of Black Feminisms](/freefeminist-resources/articles/rev_practice_black_feminism)" for a background on the history of Black feminisim in the USA. 

{% comment %}
can i generate everything tagged a certain way here.... hmm... what is feminist theory? should all articles be in the articles collection?
{% endcomment %}



