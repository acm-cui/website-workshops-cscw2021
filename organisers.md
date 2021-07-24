---
layout: page
title: Organizers

nav_text: Organizers
nav_position: 2
---


{% for organiser in site.data.organisers %}
<div class="d-flex my-5">
  <div class="flex-shrink-0">
		{%- if organiser.image -%}
		{%- assign image_path = "/assets/img/" | append: organiser.image -%}
    <img src="{{ image_path | relative_url }}" alt="An photograph of {{ organiser.name }}" class="organiser-image rounded">
		{%- else -%}
		<div class="d-block organiser-image"></div>
		{%- endif -%}
  </div>
  <div class="flex-grow-1 ms-md-5 ms-3">
    <p>
			{%- if organiser.website -%}
			<a href="{{ organiser.website }}" title="Visit {{ organiser.name }}'s website">{{ organiser.name }}</a> {{ organiser.biography }}
			{%- else -%}
			<strong>{{ organiser.name }}</strong> {{ organiser.biography }}
			{%- endif -%}
		</p>
  </div>
</div>
{% endfor %}