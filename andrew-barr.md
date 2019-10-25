---
layout: page
title: Principal Investigator
---

{% assign query = site.people | where: "family_name", "Barr" %}

{% for person in query %}
{% capture display_name %}{{person.first_name}} {{person.family_name}}{% endcapture %}
<div class="row">
<div class="col-xs-12 col-md-6">
    <h2>{{display_name}}</h2>
    <p><i class="fas fa-envelope" style="padding-right:6px"></i>wabarr@email.gwu.edu</p>
    <p>I am a paleoanthropologist and paleoecologist studying the environmental context of early human evolution.</p>

    <p>Global climate change is often framed as a major driver of human adaptation and evolution. However, despite much theorizing, we have surprisingly limited direct evidence of the impact of global climate on evolutionary events such as the origin of <i>Homo</i> and the split between the hominin and panin lineages. I conduct fieldwork and apply quantitative analytical methods in the lab aimed at filling these knowledge gaps.</p>

    <p>Currently I am exploring a new  late Miocene field site in Laikipia, Kenya, which is unique because of its geographic position outside the Great Rift Valley. I also have an active fieldwork program at Koobi Fora (Turkana Basin, Kenya) and in the Afar Region of Ethiopia (Mille-Logya). In the lab I use 3D scanning and principles of ecological functional morphology to understand the locomotor and dietary adaptations of the fauna I recover in the course of my fieldwork.</p>
</div>
<div class="col-xs-12 col-md-6">
	<img class="img-fluid rounded-circle" src="{{site.baseurl}}/{{person.headshot}}" alt='{{display_name}}'>
</div>


   
</div>
{% endfor %}
