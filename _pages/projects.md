---
title: "SAIDE PhD Project Offerings (2024 Spring cycle)"
layout: gridlay
sitemap: false
permalink: /
--- 

{% assign sorted_projects = site.data.projects | sort: "sort" %}

{% assign number_printed = 0 %}
{% for project in sorted_projects %}

<div class="row">
<h4>{{ project.title }}</h4>
{{ project.name }} <span style="float:right;"> {{ project.affiliation }} </span>
{{ project.description }}
Contact: {{ project.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}