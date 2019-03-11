---
layout: default
---

<img id="projectBanner" src="media/rgdc_logo.png"/>

RIT Game Dev club provides an open, creative, learning environment for students passionate about game development with monthly game jams and weekly presentations on topics that are voted on each week.

<!-- List of events -->
# Upcoming Events
{% for item in site.data.events %}

{% if item.title %}
### {{ item.title }}
{% endif %}

{% if item.time and item.location %}
####  {{ item.time }} in {{ item.location }}
{% endif %}

{% if item.image %}
<img id="eventBanner" src="{{ item.image }}"/>
{% endif %}

{{ item.description }}

{% endfor %} <!-- End of Event data -->