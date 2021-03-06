---
title: "Carter Lab - Publications"
layout: gridlay
excerpt: "Carter Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=nlWQnXMAAAAJ&hl=en))

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
  <img src="{{ site.url }}{{ site.baseurl }}/images/publication_pic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
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


## Full List
#### *2017*
{% for publi in site.data.publist %}
 {% if publi.year == 2017 %}
   {{ publi.title }} <br />
   <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
 {% endif %}
{% endfor %}
<br>
#### *2016*
{% for publi in site.data.publist %}
 {% if publi.year == 2016 %}
   {{ publi.title }} <br />
   <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
 {% endif %}
{% endfor %}
<br>
#### *2015*
{% for publi in site.data.publist %}
 {% if publi.year == 2015 %}
   {{ publi.title }} <br />
   <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
 {% endif %}
{% endfor %}
<br><br>
