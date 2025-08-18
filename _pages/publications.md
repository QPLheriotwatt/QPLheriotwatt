---
title: "Quantum Photonics Laboratory - Publications"
layout: gridlay
excerpt: "Quantum Photonics Laboratory -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

**Publications from the whole Quantum Photonics Lab can be found here: [QPL Google Scholar account](https://scholar.google.com/citations?hl=en&user=ses26X0AAAAJ&view_op=list_works&sortby=pubdate).**

**Publications for individual team leaders can be found on their own Google Scholar pages: [Brian Gerardot](https://scholar.google.com/citations?user=D7Z9rXcAAAAJ&hl=it&oi=ao), [Cristian Bonato](https://scholar.google.com/citations?user=u4UJsosAAAAJ&hl=it&oi=ao), [Margherita Mazzera](https://scholar.google.com/citations?user=60hNxz4AAAAJ&hl=it&oi=ao), [Mauro Brotons i Gisbert](https://scholar.google.com/citations?user=hA5Isw8AAAAJ&hl=it&oi=ao), [Christiaan Bekker](https://scholar.google.com/citations?user=d1CFpsMAAAAJ&hl=it&oi=ao), [Samer Kurdi](https://scholar.google.com/citations?user=LcsoFOQAAAAJ&hl=en&oi=ao).**

**Selected publications:**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
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

## Roadmaps and Reviews:

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
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

**We often collaborate with industry to create novel scientific instrumentations, or develop novel methodologies to exploit existing existing equipment for novel quantum experiments. This is reported in Application Notes, such as:
Zurich Instruments, [Speeding up NV Center Measurements with Real-time Control](https://www.zhinst.com/ch/en/blogs/speeding-nv-center-measurements-real-time-control).**


<!-- ## Full List of publications -->

<!-- {% for publi in site.data.publist %} -->

  <!-- {{ publi.title }} <br /> -->
  <!-- <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a> -->

<!-- {% endfor %} -->

## Talks:

