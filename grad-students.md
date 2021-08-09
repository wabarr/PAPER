---
title: Graduate Students
layout: page
---

<div class="row">
{% assign people = site.people | where: "role", "graduate student" | where: "alum", "false" | sort:"family_name" %}
{% include people_list.html %}
{% assign people = site.people | where: "role", "graduate student" | where: "alum", "true" | sort:"family_name" %}
{% include people_list.html %}
</div>
