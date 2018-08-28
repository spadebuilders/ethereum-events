---
layout: single
title: Calendar
permalink: /calendar/
---

<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.9.0/fullcalendar.min.css">
<link rel="stylesheet" media="print" href="//cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.9.0/fullcalendar.print.css">

<script>
$(function() {

	$('#fullcalendar').fullCalendar({
		events:'/events/json'
	})

});
</script>

<div id="fullcalendar">
<noscript>Full Calendar needs JavaScript Enabled</noscript>
</div>