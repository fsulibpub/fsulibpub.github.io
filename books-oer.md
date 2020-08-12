---
layout: default
title: Books and Textbooks 
permalink: /books-oer/
---

{% for page in site.books-oer %}
  <img class="preview" src="{{ site.baseurl }}/assets/images/{{ page.image }}">
  <section class="description"><h2><a href="{{ site.baseurl }}{{ page.permalink }}">{{ page.title }}</a></h2>
  <p>{{ page.description }}</p>
  </section>
{% endfor %}