---
layout: page
title:  "Central Bands"
date:   2019-02-06 10:37:00 +0000
categories: central-bands
permalink: /:categories
---

Further analysis of the networks displayed in my [Band Maps post](https://tobyjdore.github.io/band-maps).

These are the [betweenness centralities](https://en.wikipedia.org/wiki/Betweenness_centrality){:target="blank"} for all of the bands in the main band's network (where equal to or greater than 0.01 for sanity's sake).

Read the project report [here](https://tobyjdore.github.io/how-i-wrote-band-maps).

{% for image in site.static_files %}
    {% if image.path contains 'images/centrality-plots' %}
<div class="cropthumbcontainer">
  <a href="{{ site.baseurl }}{{ image.path }}"><img src="{{ site.baseurl }}{{ image.path }}" width="200" height="200" alt="{{ image.title }}">
  <div class="centered"><h2>{{ image.basename | replace: "-", " " | replace: "btwn", ""}}</h2></div></a>
</div>
    {% endif %}
{% endfor %}

<p style="clear: both;">
