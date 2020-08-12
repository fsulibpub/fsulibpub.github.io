---
layout: default 
title: "News and Updates"
permalink: /news/
---

{% assign news_by_date = site.news | sort = "date" | reverse %}
{% for news in news_by_date %}
<h3><a href="{{ news.permalink }}">{{ news.title }}</a></h3>
{{ news.content | truncate: 200 }} <a href="{{ news.permalink }}">[read more]</a><br/>
<em>{{ news.date }}</em>
{% endfor %}