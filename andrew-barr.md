---
layout: page
title: W. Andrew Barr
---

{% assign query = site.people | where: "family_name", "Barr" %}

{% for person in query %}
{% capture display_name %}{{person.first_name}} {{person.family_name}}{% endcapture %}
<div class="row">
<div class="col-xs-12 col-md-6">
	<img class="img-fluid" src="{{site.baseurl}}/{{person.headshot}}" alt='{{display_name}}'>
    
    <p style='padding-top:15px'>I am a paleoanthropologist and paleoecologist studying the environmental context of early human evolution.</p>

    <p>Global environmental change is often framed as a major driver of human adaptation and evolution. However, despite much theorizing, we have surprisingly limited direct evidence of the impact of global change on evolutionary events such as the origin of <i>Homo</i> and the split between the hominin and panin lineages. I conduct fieldwork and apply quantitative analytical methods in the lab aimed at filling these knowledge gaps.</p>

	<p>The <a href="/projects/">projects page</a> provides more detail on currently active projects in the PAPER lab. </p>
	<p><i class="fas fa-envelope" style="padding-right:6px"></i>wabarr@email.gwu.edu</p>
	
</div>


<div class="col-xs-12 col-md-6">
	{% include barr-CV.html %}
</div>


   
</div>
{% endfor %}
