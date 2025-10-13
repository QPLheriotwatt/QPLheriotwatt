---
title: "Quantum Photonics Laboratory - Pictures"
layout: piclay
excerpt: "Quantum Photonics Laboratory -- Pictures"
permalink: /pictures/
---

# Pictures

<div style="font-size:1.2em">
Click on the categories to see the corresponding pictures.

(Right-click ‘open image in new tab’ to see a larger image.)
</div>

{% assign galleries = "TeamBuilding,GroupPhotos,Outreach" | split: "," %}

{% for gallery_folder in galleries %}
<details>
<summary><h2>{{ gallery_folder | replace: "Team", "Team " | replace: "Group", "Group " }}</h2></summary>

{% assign number_printed = 0 %}
{% for file in site.static_files %}

{% assign target_path = "/images/1_TeamBuilding_Social/" | append: gallery_folder %}
{% if file.path contains target_path %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-3 clearfix">
<div style="margin-bottom: 5px; overflow: hidden;">
<img src="{{ site.baseurl }}{{ file.path }}" class="img-responsive" width="100%" style="display: block; margin: 0 auto;" />
</div>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 3 %}
</div>
{% endif %}
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
</details>
{% endfor %}