---
title: "Quantum Photonics Laboratory - News"
layout: piclay
excerpt: "Heriot-Watt University"
sitemap: false
permalink: /allnews.html
---

# News

Click on the news headlines to see more information.

{% for article in site.data.news %}

<details><summary><h4>**{{ article.date }} - {{ article.headline }}** </h4></summary>
{% if article.details %}
{{ article.details | markdownify}}
{% endif %}
</details>

{% endfor %}
