---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<img align="left" width="200" style="margin-right: 10px" src="{{ site.url }}/images/project-sort.mp4" alt="...">
GelTip: A Finger-shaped Optical Tactile Sensor for Robotic Manipulation <br />
D.F. Gomes, Z. Lin, **S. Luo**. IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 2020. <br />
[[paper]](https://arxiv.org/abs/2008.05404) [[website]](https://danfergo.github.io/geltip/) [[STL files]](https://danfergo.github.io/geltip/geltip2020_parts.zip)