---
layout: home
title: Appli
date: 2016-04-01
categories: ["Onderwijs"]
techniques:
    - "PHP"
    - "Symfony"
    - "Doctrine ORM"
    - "PHPUnit"
    - "PHP Codestyle Fixer"
    - "PostgreSQL"
    - "MySQL"
    - "SQLite"
    - "Redis"
    - "Composer"
    - "Git"
    - "Jira"
    - "Bitbucket"
logo:
    url: /img/logo-appli.png
    title: Appli
    alt: Logo Appli
summary: Appli is een app (voor iOS en Android) om studenten en stageplekken te
    matchen. Op een Tinder-achtige manier (swipen, liken en super-liken) worden
    bedrijven met stage-vacatures gekoppeld aan studenten die op zoek zijn naar
    een stageplek.
me: Voor dit project was ik in de rol van lead developer verantwoordelijk voor
    de ontwikkeling van webservices met RESTful API, die de schakel vormen
    tussen de apps en de database.
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
