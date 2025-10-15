---
title: "Quantum Photonics Laboratory - Outreach"
layout: gridlay
excerpt: "Quantum Photonics Laboratory -- Outreach"
sitemap: false
permalink: /outreach/
---

## Blogs:
{% assign number_printed = 0 %}
{% for publi in site.data.bloglist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well" style="min-height: 200px; overflow: hidden;">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/blogpic/{{ publi.image }}" class="img-responsive" width="40%" style="float: left; margin-right: 15px; margin-bottom: 10px;" />
  <div style="overflow: hidden;">
   <p>{{ publi.description }}</p>
   <p><em>{{ publi.authors }}</em></p>
   <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
   <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
   <p> {{ publi.news2 }}</p>
  </div>
  <div style="clear: both;"></div>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Podcasts:

**Under the Microscope - Atomic Architects: Designing the Future of Quantum ft. Brian Gerardot**
<iframe width="560" height="315" src="https://www.youtube.com/embed/6GbR_X6_yJQ" frameborder="0" allowfullscreen></iframe>

**Quantum Magnetic Materials Podcast - Episode 1 - General Introduction**
<iframe width="560" height="315" src="https://www.youtube.com/embed/2R3C9HVS-Jk" frameborder="0" allowfullscreen></iframe>


## Talks:
**Scottish Universities Physics Alliance (SUPA) – Public Engagement Forum: HWU–TEDxCesena Adventure, The Secrets of Light ft. Margherita Mazzera**

<iframe width="560" height="315" src="https://www.youtube.com/embed/Op5YNQIyzgc" frameborder="0" allowfullscreen></iframe>

**TEDx: E se la meccanica quantistica fosse divertente? ft. Margherita Mazzera**

<iframe width="560" height="315" src="https://www.youtube.com/embed/MM1pus_Y0Cc" frameborder="0" allowfullscreen></iframe>

