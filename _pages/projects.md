---
title: "SAIDE PhD Project Offerings (2024 Spring cycle)"
layout: gridlay
sitemap: false
permalink: /
--- 

{% assign sorted_projects = site.data.projects | sort: "name" %}
{% assign sorted_projects = sorted_projects | sort: "affiliation" %}
{% assign sorted_projects = sorted_projects | sort: "sort" %}

{% assign number_printed = 0 %}
{% for project in sorted_projects %}

<div class="row nb">
<h4>{{ project.title }}</h4>
<p>{{ project.name }} <span style="float:right;"> {{ project.affiliation }} </span></p>
<p>{{ project.description | replace: "  ", "  \n" }}</p>
<p>Contact: [{{ project.email }}](mailto:{{ project.email }})</p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}