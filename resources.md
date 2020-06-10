---
layout: default
title: Resources
description: Other useful resources from across the internet
permalink: /resources/
tags:
  - "Africa"
  - "African diaspora"
  - "Collaboration"
  - "Dance"
  - "Ethnomusicology"
  - "Historical Ethnomusicology"
  - "Indigeneity"
  - "Jazz"
  - "Latin America"
  - "Media"
  - "Native America"
  - "Popular Music"
  - "Sound"
  - "Teaching"
  - "Virtual Fieldwork"
---

One of our goals is to provide links to some of the many open and online resources available online that are related to the teaching and study of world music. These are not exhaustive, but may provide starting points for research or reading. If you would like to add any resources or suggest a bibliography, please email [Christopher Witulski][email].

## Filter by tag

<div>
    {% assign sorted-tags = (page.tags | sort) %}
    {% for tag in sorted-tags %}
        <span id="{{ tag }}" class="tag btn">{{ tag }}</span>
    {% endfor %}
</div>

## Resources

<div>
    {% for bib in site.resources %}
        {% assign sorted-pubs = (bib.resources | sort:'date' | reverse) %}
        {% for pub in sorted-pubs %}
            {% include item.html pub=pub %}
        {% endfor %}
    {% endfor %}
</div>

[email]: mailto:cwituls@bgsu.edu
