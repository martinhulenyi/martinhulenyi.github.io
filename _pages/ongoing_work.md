---
title: "Ongoing work"
permalink: /ongoing_work/
author_profile: true
layout: archive
---

{% include base_path %}

{% for post in site.ongoing_work reversed %}
  {% include archive-single.html type="list" %}
{% endfor %}
