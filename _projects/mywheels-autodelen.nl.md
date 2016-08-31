---
layout: home
title: MyWheels
date: 2014-05-01
categories: ["Milieu & Duurzaamheid", "Deeleconomie"]
techniques:
	- "PHP"
	- "Symfony"
	- "Doctrine ORM"
    - "PHPUnit"
    - "PHP Codestyle Fixer"
    - "PostgreSQL"
    - "MySQL"
    - "SQLite"
	- "Composer"
	- "Git"
	- "Jira"
	- "Github"
logo:
    url: /img/logo-mywheels.png
    title: MyWheels
    alt: Logo MyWheels
summary: MyWheels is een not-for-profit platform voor autodelen dat als ideaal
    heeft om mensen een bewuste keuze te laten maken voor elke autorit.
    Soms is een auto de beste optie om van A naar B te komen, maar vaak is
    een (OV-)fiets of de trein een beter alternatief. Met autodelen worden
    autokosten variabel - je betaalt alleen als je rijdt - en kun je vaker voor
    een duurzaam alternatief kiezen.
me: Voor MyWheels maakte ik deel uit van een klein team van software-ontwikkelaars.
    Ik werkte mee aan de backend, de motor achter dit online platform. Ik bouwde
    ondermeer modules voor facturatie, betaling, kortings- en tegoedbonnen, koppelingen
    met
---
<div class="row">
    <div class="col-xs-12">
        <h2>{{ page.title }}</h2>
        <img src="{{ page.logo.url }}" title="{{ page.logo.title }}" alt="{{ page.logo.alt }}" class="img-responsive pull-right">
        <p>{{ page.summary }}</p>
        <p>{{ page.me }}</p>
        <ul class="list-inline">
        {% for technique in site.techniques %}
            {% if page.techniques contains technique.title %}
                <li>
                    <a href="{{ technique.url }}">
                        <span class="label label-default">{{ technique.title }}</span>
                    </a>
                </li>
            {% endif %}
        {% endfor %}
        </ul>
    </div>
</div>
