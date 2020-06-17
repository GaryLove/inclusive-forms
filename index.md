---
layout: front.liquid
pageTitle: Front page
---
{% for best-practice in collections.best-practices %}
<h2><a href="{{ best-practice.url }}">{{ best-practice.data.pageTitle }}</a></h2>
<em>{{ best-practice.date | date: "%Y-%m-%d" }}</em>
{% endfor %}