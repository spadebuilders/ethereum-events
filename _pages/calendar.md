---
layout: single
title: Calendar
permalink: /calendar/
head_scripts:
 - /assets/js/moment.min.js
 - https://code.jquery.com/jquery-3.3.1.min.js
 - https://code.jquery.com/ui/1.12.1/jquery-ui.min.js
 - https://cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.9.0/fullcalendar.min.js

---

<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.9.0/fullcalendar.min.css">
<link rel="stylesheet" media="print" href="//cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.9.0/fullcalendar.print.css">

<script>
$(document).ready(function() {

	$('#calendar').fullCalendar({
		events:'/events/json'
	})

});
</script>

<div id="calendar"></div>