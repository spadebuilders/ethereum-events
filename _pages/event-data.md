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
		{% assign eventstart = event.event.start_date | date: "%Y-%m-%dT%H:%M%z" %}
		{% assign eventend = event.event.end_date | date: "%Y-%m-%dT%H:%M%z" %}
		{% assign eventstartday = event.event.start_date | date: "%Y-%m-%d" %}
		{% assign eventendday = event.event.end_date | date: "%Y-%m-%d" %}
	{
		"title": "{{event.title}}",
		"start": "{{ eventstart }}",
		"end": "{{ eventend }}",
		"url": "{{ eventlink }}"{% if eventstartday != eventendday %},
    "allDay": true{% endif %}
	}{%unless forloop.last %},{%endunless%}
{% endfor %}
]