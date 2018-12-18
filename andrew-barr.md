---
layout: page
title: Principal Investigator
---

{% assign PIs = site.people | where: "role", "PI" %}


{% comment %} sanity check to make sure no accidental PIs get added {% endcomment %}

{% if PIs.size == 1 %}
{% for barr in PIs %}
<div class="row">
<div class="col-xs-12 col-md-6">
   <h2>W. Andrew Barr</h2>
   
   <p>I am a paleoanthropologist and paleoecologist interested in understanding the environmental context of early human evolution.</p>

   <p>Global climate change is often framed as a major driver of human adaptation and evolution. However, despite much theorizing, we have surprisingly limited direct evidence of the impact of global climate on evolutionary events such as the origin of <i>Homo</i> and the split between the hominin and panin lineages. I conduct fieldwork and apply quantitative analytical methods in the lab aimed at filling these knowledge gaps.</p>

   <p>Currently I am exploring a new  late Miocene field site in Laikipia, Kenya, which is unique because of its geographic position outside the Great Rift Valley. I also have an active fieldwork program at Koobi Fora (Turkana Basin, Kenya) and in the Afar Region of Ethiopia (Mille-Logya). In the lab I use 3D scanning and principles of ecological functional morphology to understand the locomotor and dietary adaptations of the fauna I recover in the course of my fieldwork.</p>
</div>
<div class="col-xs-12 col-md-6">
   <img class="img-fluid rounded-circle" src="{{site.baseurl}}/{{barr.headshot}}" alt="W. Andrew Barr">
</div>
</div>
{% endfor %}
{% endif %}
