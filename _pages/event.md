---
layout: archive
title: Events Archive
permalink: /events/
sidebar:
  - text: "<a href='/add'>Add your event</a>"
---

{% assign entries = site.events | sort: 'event.start_date' | reverse %}
{% assign buildtime = "now" | date: '%s' %}
{% for post in entries %}
  {% assign startdate = post.event.start_date | date: '%s' %}
  {% if startdate < buildtime %}
    {% include event-single.html %}
  {% endif %}
{% endfor %}