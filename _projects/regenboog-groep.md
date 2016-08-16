---
layout: project
title: Regenboog Groep
date: 2015-11-01
categories: ["Welzijn"]
techniques: ["advies", "begeleiding", "PHP", "CakePHP", "MySQL", "open source"]
logo:
    url: /img/logo-regenboog-groep.png
    title: Regenboog Groep
    alt: Logo Regenboog Groep
summary: Voor De Regenboog Groep begeleid ik de ontwikkeling van een elektronisch
    cliëntendossier. Dit is een online applicatie waarin de zorg aan cliënten
    wordt geregistreerd. Mijn rol bestaat uit het adviseren over het ontwikkeltraject
    en het maken van de vertaalslag van gebruikerswensen naar technische specificaties.
    Daarvoor ben ik voortdurend in gesprek met zowel de eindgebruikers binnen de organisatie
    als de programmeurs van een extern software-bureau.
---
<div class="row odd">
    <ol class="breadcrumb">
        <li><a href="/">Home</a></li>
        <li><a href="/projecten/">Projecten</a></li>
        <li class="active">{{ page.title }}</li>
    </ol>
    <div class="col-xs-12">
        <img class="img-responsive pull-right" src="{{ page.logo.url }}"/>
        <h1>{{ page.title }}</h1>
    <strong>{{ page.summary }}</strong>
    <ul>
    {% for technique in site.techniques %}
        {% if page.techniques contains technique.title %}
            <li><a href="{{ technique.url }}">{{ technique.title }}</a></li>
        {% endif %}
    {% endfor %}
    </ul>
    </div>
</div>
