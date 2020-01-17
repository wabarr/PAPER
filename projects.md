---
title: Current Projects
layout: page
---

<div class="row">
	
		{% for project in site.data.projects %}
		<div class="col-xs-12 col-md-6 ">
			<h2>{{project.name}}</h2>
			<p>{{project.description}}</p>
		</div>
		{% endfor %}
	
</div>