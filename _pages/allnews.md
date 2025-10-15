---
title: "Quantum Photonics Laboratory - News"
layout: piclay
excerpt: "Heriot-Watt University"
sitemap: false
permalink: /allnews/
---

# News

Click on the news headlines to see more information.

{% for article in site.data.news %}

<details markdown="1">
<summary><h4 style="display: inline;"><strong>{{ article.date }} – {{ article.headline }}</strong></h4></summary>

<div markdown="1">
{% if article.details %}
{{ article.details | markdownify }}
{% endif %}
</div>

{% if article.photos %}
<div class="row">
  {% for photo in article.photos %}
  <div class="col-sm-4">
    <img src="{{ '/images/newspic/' | relative_url }}{{ photo.filename }}" alt="{{ photo.alt | default: '' }}" class="img-responsive" style="max-height: 250px; margin: 0 auto;">
    {% if photo.caption %}
    <div style="text-align: center; margin-top: 5px;">
      <strong>{{ photo.caption }}</strong>
    </div>
    {% endif %}
  </div>
  {% endfor %}
</div>
{% endif %}

{% if article.video %}
<div class="row">
  <div class="col-sm-8 col-sm-offset-2">
    <div class="embed-responsive embed-responsive-16by9">
      <video controls class="embed-responsive-item">
        <source src="{{ '/images/newspic/' | relative_url }}{{ article.video }}" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
  </div>
</div>
{% endif %}

</details>

{% endfor %}

<style>
details > summary {
  cursor: pointer;
  padding: 10px;
  background-color: #f5f5f5;
  border-radius: 5px;
  margin-bottom: 10px;
}
details > div {
  padding: 15px;
}
details {
  margin-bottom: 20px;
}
</style>
