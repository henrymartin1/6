---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Welcome!
I am currently pursuing a doctoral degree at the [Chair of Geoinformation Engineering](https://gis.ethz.ch/en/) at ETH Zurich. I am supervised by [Martin Raubal](http://www.raubal.ethz.ch/) and work in the Mobility Information Engineering Lab ([MIE-Lab](http://mie-lab.ethz.ch/)). Since 2020 I am also a research fellow at the Institute of [Advanced Research in Artificial Intelligence](https://www.iarai.ac.at/) (IARAI) in Vienna. 

I am interested in sustainability of human mobility and energy systems, network science and machine learning.


# News

{% capture written_year %} 'None' {% endcapture %}
{% for post in site.posts -%}
  {%- capture year -%}{{ post.date | date: '%Y' }}{% endcapture %}
  {%- if year != written_year -%}
     <h2>{{ year }}</h2>
    {%- capture written_year -%}{{- year -}}{%- endcapture -%}
  {% endif -%}
  * {{ post.title }} [[more...]({{- post.permalink -}})]
{% endfor %}