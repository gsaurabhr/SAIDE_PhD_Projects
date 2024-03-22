---
title: "SAIDE PhD Project Offerings (2024 Spring cycle)"
layout: gridlay
sitemap: false
permalink: /projects/
--- 
{% assign number_printed = 0 %}
{% for project in sorted_prjects %}

<div class="col-sm-12 clearfix" markdown="1">
<h4>{{ project.title }}</h4>
{{ project.name }} <span style="float:right;"> {{ project.affiliation }} </span>
{{ project.description }}
Contact: {{ project.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}