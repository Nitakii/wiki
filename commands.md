---
title: Commands
layout: default
permalink: /commands
---

# Commands

Im Folgenden findet ihr eine Auflistung aller Commands auf Farmlife: Badoras
(ohne Garantie auf Vollständigkeit).

<table>
	<tr>
		<th>
			Command
		</th>
		<th>
			Beschreibung
		</th>
	</tr>
	{% for command in site.commands %}
	<tr>
		<td>
			<center><pre>/{{ command.command }}</pre></center>
		</td>
		<td>
			<center>{{ command.content }}</center>
		</td>
	</tr>
	{% endfor %}
</table>
