---
title: Online gehostete Anweisungen
permalink: index.html
layout: home
---

# Inhaltsverzeichnis

Hyperlinks zu den Lab-Übungen und Demos sind nachfolgend aufgelistet.

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Modul | Übungen |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

## Demos

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| Modul | Demos |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
