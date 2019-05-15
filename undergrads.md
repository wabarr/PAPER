---
title: Undergraduate Researchers
layout: page
---

<div class="row">
{% assign people = site.people | where: "role", "undergraduate researcher" | sort:"family_name" %}
{% include people_list.html %}
</div>