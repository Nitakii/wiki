---
title: Team
layout: default
permalink: /team
nav_order: 3
---

# Alle Teammitglieder

{% for team_member in site.team_members %}
{% if team_member.section == "misc" %}
{: .text-purple-000 }
{% endif %}
{% if team_member.section == "admin" %}
{: .text-red-300 }
{% endif %}
{% if team_member.section == "team" %}
{: .text-yellow-300 }
{% endif %}
{% if team_member.section == "support" %}
{: .text-blue-000 }
{% endif %}
<h2> {{ team_member.name }} - {{ team_member.position }} </h2>
{{ team_member.content | markdownify }}
{% if team_member.responsibilities %}
<b>Verantwortlich für:</b>
<ul>
{% for responsibility in team_member.responsibilities %}
<li> {{ responsibility }} </li>
{% endfor %}
</ul>
{% endif %}
{% if team_member.contributions %}
<b>Beteiligt an:</b>
<ul>
{% for contribution in team_member.contributions %}
<li> {{ contribution }} </li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
