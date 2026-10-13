---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

I am a PhD candidate in Electronic Science and Technology at the [Advanced Neural Chip Center](https://www.westlake.edu.cn), Westlake University, advised by [Prof. Mohamad Sawan](https://www.westlake.edu.cn) (Fellow of the Canadian Academy of Engineering, IEEE Life Fellow). I received my BEng in Microelectronics Science and Engineering from Fudan University in 2022.

My research focuses on **neuromorphic computing and brain-inspired chip design**. I work on ultra-low-power digital neuromorphic processors for edge-side perception, covering the full flow from architecture and circuit design to 28nm tape-out and silicon validation. Application areas include 3D point-cloud recognition, spiking vision transformers, and neuromorphic sensing for autonomous driving and embodied intelligence.

Publications
======

Newest first. Full list with abstracts on the [publications page]({{ base_path }}/publications/).

{% for post in site.publications reversed %}
* **{{ post.date | date: "%Y" }}** &mdash; Our work *"[{{ post.title }}]({{ base_path }}{{ post.url }})"* has been published in *{{ post.venue }}*.{% if post.paperurl %} [[paper]]({{ post.paperurl }}){% endif %}

{% endfor %}
