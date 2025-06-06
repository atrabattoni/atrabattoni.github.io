---
permalink: /instruments/
title: "Instruments"
---

Explore our curated collection of scientific instruments available for borrowing. Whether you're conducting research, teaching, or pursuing a personal project, these tools are here to support your scientific endeavors. Browse the list below to find detailed information, images, and descriptions for each instrument.

<ul>
  {% for instrument in site.instruments %}
    <li style="margin-bottom: 2em;">
      <a href="{{ instrument.url }}">
        <img src="{{ instrument.thumbnail }}" alt="Thumbnail for {{ instrument.title }}" style="width: 150px; height: auto; float: left; margin-right: 1em;" />
        <h2>{{ instrument.title }}</h2>
      </a>
      <p>{{ instrument.short_description }}</p>
      <div style="clear: both;"></div>
    </li>
  {% endfor %}
</ul>
