---
title: "Quantum Photonics Laboratory - News"
layout: textlay
excerpt: "Heriot-Watt University"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
**{{ article.date }}** - **{{ article.headline }}**
{% if article.details %}
{{ article.details | markdownify}}
{% endif %}

{% endfor %}
