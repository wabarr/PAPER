---
layout: page
title: Principal Investigator
---

{% assign PIs = site.people | where: "role", "PI" %}


{% comment %} sanity check to make sure no accidental PIs get added {% endcomment %}

{% if PIs.size == 1 %}
{% for barr in PIs %}
<div class="row">
<div class="col-s12 col-md-8">
   <h2>W. Andrew Barr</h2>
   <img class="img-fluid" src="{{site.baseurl}}/{{barr.headshot}}" alt="W. Andrew Barr">
</div>
</div>
{% endfor %}
{% endif %}
