---
layout:
title:
permalink: /events/json
---
[
{% for event in site.events %}
		{% if event.link %}
		  {% assign eventlink = event.link %}
		{% else %}
		  {% assign eventlink = event.url %}
		{% endif %}
	{
		"title":"{{event.title}}",
		"start": "{{event.event.start_date}}",
		"end": "{{event.event.end_date}}",
		"allDay":true,
		"url":"{{ eventlink }}"
	}
	{%unless forloop.last %},{%endunless%}
{% endfor %}
]