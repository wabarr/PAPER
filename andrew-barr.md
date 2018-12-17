---
layout: page
title: Principal Investigator
---

<div class="row">
{% assign people = site.people | where: "role", "PI" %}
{% include people_list.html %}
</div>