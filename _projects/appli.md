---
layout: default
title: Appli
date: 2016-04-01
categories: ["Onderwijs"]
techniques: ["PHP", "Symfony", "Doctrine", "PHPUnit", "MySQL", "PostgreSQL", "SQLite", "Redis", "Composer", "Git", "Jira", "Bitbucket"]
logo:
    url: /img/logo-appli.png
    title: Appli
    alt: Logo Appli
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque vel velit diam. Nunc accumsan, urna in ornare cursus, quam risus dapibus erat, vel efficitur felis magna molestie orci. Pellentesque risus arcu, malesuada ac odio et, tincidunt mattis est. Etiam justo ligula, pulvinar eu convallis eu, semper vitae velit. Nullam at cursus felis. Fusce eget vestibulum turpis, quis pellentesque est. Nunc in volutpat est. Fusce laoreet, mi in suscipit semper, turpis nisl condimentum lorem, quis facilisis erat urna et augue. Vestibulum cursus vestibulum purus, in mattis quam elementum non. Pellentesque lacinia sagittis orci, eget ultricies odio. Ut vitae iaculis felis. Suspendisse potenti. Morbi facilisis ex in dolor accumsan pellentesque. Suspendisse eu elit metus. Nunc tincidunt tortor a nunc vulputate, id commodo magna porta.
---
![Logo Appli](/img/logo-appli.png "Appli")

# {{ page.title }}

Appli is een (iOS en Android) app om studenten en stageplekken bij elkaar te
brengen. Op een Tinder-achtige manier (swipen, liken en super-liken) worden
matches gemaakt tussen bedrijven die een stageplek aanbieden en studenten die
daarnaar op zoek zijn.

Voor dit project ontwikkelde ik op basis van het Symfony-framework de
[REST API](https://en.wikipedia.org/wiki/Representational_state_transfer)
waarmee de apps communiceren.

<ul>
{% for technique in site.techniques %}
    {% if page.techniques contains technique.title %}
        <li><a href="{{ technique.url }}">{{ technique.title }}</a></li>
    {% endif %}
{% endfor %}
</ul>
