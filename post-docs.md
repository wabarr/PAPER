---
title: Postdoctoral Researchers
layout: page
---

<div class="row">
{% assign people = site.people | where: "role", "postdoc" | where: "alum", "false" | sort:"family_name" %}
{% include people_list.html %}
{% assign people = site.people | where: "role", "postdoc" | where: "alum", "true" | sort:"family_name" %}
{% include people_list.html %}
</div>