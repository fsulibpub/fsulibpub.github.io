---
layout: default
title: Journals 
permalink: /journals/
---

{% for page in site.journals %}
  <img class="preview" src="{{ site.baseurl }}/assets/images/{{ page.image }}">
  <section class="description"><h2><a href="{{ site.baseurl }}{{ page.permalink }}">{{ page.title }}</a></h2>
  <p>{{ page.description }}</p>
  </section>
{% endfor %}