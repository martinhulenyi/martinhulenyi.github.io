---
title: "Ongoing work"
permalink: /ongoing_work/
author_profile: true
layout: archive
---

{% include base_path %}

{%- assign jmp_items = site.ongoing_work | where: "jmp", true | sort: "date" | reverse -%}
{%- assign other_items = site.ongoing_work | where_exp: "p", "p.jmp != true" | sort: "date" | reverse -%}

{%- for post in jmp_items -%}
  {% include archive-single.html type="list" %}
{%- endfor -%}

{%- for post in other_items -%}
  {% include archive-single.html type="list" %}
{%- endfor -%}
