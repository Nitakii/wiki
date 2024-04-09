---
title: Support
layout: default
permalink: /support
nav_order: 4
---
# Support

Du kommst einmal nicht weiter, trotz aller Informationen im Wiki oder unter
`/hilfe`? Kein Problem, dafür ist unser kompetentes Support-Team gerne zur
Stelle.

Nebenbei haben unsere Supporter auch die Aufgabe, über die Einhaltung des
Regelwerks zu wachen. Hierbei kommt ein spezielles Punktesystem zur Geltung.

## Kontaktmöglichkeiten

Unser Support kann auf verschiedenen Wegen erreicht werden:
- Auf [Discord](https://discord.gg/Fx2pUMCejP) per Community-Support.
- Auf [Discord](https://discord.gg/T9HEBpGazE) per Ticket.
- Ingame; mehr Informationen hierzu folgen noch.

{: .note }
Generell empfiehlt es sich, erst die Möglichkeiten des Communitysupports zu
nutzen. Bei vielen Fragen können vermutlich andere Spieler\*innen (schneller!)
helfen.

## Punktesystem

Informationen hierzu werden demnächst ergänzt.

## Unser Support-Team

{% for team_member in site.team_members %}
{% if team_member.section == "support" %}
{: .text-blue-000 }
{% else %}
{% continue %}
{% endif %}
<h3> {{ team_member.name }} - {{ team_member.position }} </h3>
{{ team_member.content | markdownify }}
{% endfor %}
{% for helper in page.helpers %}
{: .text-blue-000 }
<h3> {{ team_member.name }} - {{ team_member.position }} </h3>
{{ team_member.content | markdownify }}
{% endfor %}
