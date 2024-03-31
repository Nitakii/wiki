---
title: Team
layout: default
permalink: /team
nav_order: 3
---

# Alle Teammitglieder
{% assign pos_Genius = site.team_members | where: 'position', "Genius" %}
{% for team_member in pos_Genius %}
  <h2>{{ team_member.name }} - {{ team_member.position }}</h2>
  {: .text-purple-000 }
  <p>{{ team_member.content | markdownify }}</p>
{% endfor %}
{% assign pos_Serverleitung = site.team_members | where: 'position', "Serverleitung" %}
{% for team_member in pos_Serverleitung %}
  <h2>{{ team_member.name }} - {{ team_member.position }}</h2>
  {: .text-red-300 }
  <p>{{ team_member.content | markdownify }}</p>
{% endfor %}
{% assign pos_Moderation = site.team_members | where: 'position', "Moderation" %}
{% for team_member in pos_Moderation %}
  <h2>{{ team_member.name }} - {{ team_member.position }}</h2>
  {: .text-yellow-300 }
  <p>{{ team_member.content | markdownify }}</p>
{% endfor %}
{% assign pos_Support-Leitung = site.team_members | where: 'position', "Support-Leitung" %}
{% for team_member in pos_Support-Leitung %}
  <h2>{{ team_member.name }} - {{ team_member.position }}</h2>
  {: .text-blue-000 }
  <p>{{ team_member.content | markdownify }}</p>
{% endfor %}
{% assign pos_Support = site.team_members | where: 'position', "Support" %}
{% for team_member in pos_Support %}
  <h2>{{ team_member.name }} - {{ team_member.position }}</h2>
  {: .text-blue-000 }
  <p>{{ team_member.content | markdownify }}</p>
{% endfor %}
