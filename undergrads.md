---
title: Undergraduate Researchers
layout: page
---

<div class="row">
{% assign people = site.people | where: "role", "undergraduate researcher" | where: "alum", "false" | sort:"family_name" %}
{% include people_list.html %}
{% assign people = site.people | where: "role", "undergraduate researcher" | where: "alum", "true" | sort:"family_name" %}
{% include people_list.html %}
</div>