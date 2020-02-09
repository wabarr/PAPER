---
layout: page
title: W. Andrew Barr
---

{% assign query = site.people | where: "family_name", "Barr" %}

{% for person in query %}
{% capture display_name %}{{person.first_name}} {{person.family_name}}{% endcapture %}
<div class="row">
<div class="col-xs-12 col-md-6">
	<img class="img-fluid rounded-circle" src="{{site.baseurl}}/{{person.headshot}}" alt='{{display_name}}'>
    
    <p style='padding-top:15px'>I am a paleoanthropologist and paleoecologist studying the environmental context of early human evolution.</p>

    <p>Global environmental change is often framed as a major driver of human adaptation and evolution. However, despite much theorizing, we have surprisingly limited direct evidence of the impact of global change on evolutionary events such as the origin of <i>Homo</i> and the split between the hominin and panin lineages. I conduct fieldwork and apply quantitative analytical methods in the lab aimed at filling these knowledge gaps.</p>

	<p>The <a href="/projects/">projects page</a> provides more detail on currently active projects in the PAPER lab. </p>
	<p><i class="fas fa-envelope" style="padding-right:6px"></i>wabarr@email.gwu.edu</p>
</div>


<div class="col-xs-12 col-md-6">
	

	<object data="{{site.CVlink}}" type="application/pdf" width="100%" height="100%">
	<iframe src={{site.CVlink}} width="100%" height="100%" style="border: none;">
	This browser does not support embedded PDFs. Please download the PDF to view it: <a href="{{page.CVlink}}">Download PDF</a>
	</iframe>
	</object>
	<a href="{{site.CVlink}}">Download CV as PDF</a><br>
</div>


   
</div>
{% endfor %}
