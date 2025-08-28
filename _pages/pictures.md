---
title: "Quantum Photonics Laboratory - Pictures"
layout: piclay
excerpt: "Quantum Photonics Laboratory -- Pictures"
permalink: /pictures/
---

# Pictures


## Team building & Socials

<!-- #### Timelapse of our STM assembling [(see LION news item)](https://www.physics.leidenuniv.nl/index.php?id=11573&news=867&type=lion&ln=EN): -->
<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/3iKvUMv1h5A" frameborder="0" allowfullscreen></iframe> -->

<!-- #### Gallery -->
(Right-click 'view image' to see a larger image.)


{% assign number_printed = 0 %}
{% for pic in site.data.socials %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-3 clearfix">
<div style="margin-bottom: 15px; overflow: hidden;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/socials/{{ pic.image }}" class="img-responsive" width="100%" style="display: block; margin: 0 auto;" />
  {% if pic.title %}
  <p class="text-center"><em>{{ pic.title }}</em></p>
  {% endif %}
</div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Outreach
<!-- From the [group of Felix Baumberger](http://dqmp.unige.ch/baumberger/) (now at University of Geneva). -->
{% assign number_printed = 0 %}
{% for pic in site.data.outreach %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<div style="margin-bottom: 15px; overflow: hidden;">
<img src="{{ site.url }}{{ site.baseurl }}/images/outreach/{{ pic.image }}" class="img-responsive" width="100%" style="display: block; margin: 0 auto;" />
{% if pic.title %}
<p class="text-center"><em>{{ pic.title }}</em></p>
{% endif %}
</div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>