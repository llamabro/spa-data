---
layout: page
title: Sketches
permalink: /sketches/
---
### Sample displays of musical ideas from Prokofiev's notebooks.

Playable transcriptions encoded in [MEI](https://music-encoding.org/) and displayed with [Verovio](https://www.verovio.org/index.xhtml)

(MEI and MusicXML files [available here](../data-files))

<!-- Verovio document collection -->
<H1>{{ verovio.name }}</H1>
<ul>
  {% for item in site.midi %}
    <li>
      <h4><a href="{{ site.baseurl }}/midi/{{ item.shortname }}/">{{ item.name }}</a></h4>
    </li>
  {% endfor %}
</ul>

<ul>
  {% for item in site.midi %}
  <li>
  <h3>{{ item.name }} - {{ item.imgfile }}</h3>

  <p><a href="{{ site.baseurl }}/_midi/{{ item.shortname }}/">underscore link</a></p>
  </li>
  {% endfor %}
</ul>  
