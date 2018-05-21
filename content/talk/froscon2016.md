+++
title = "Docker Container orchestrieren mit Rancher"
date = 2018-05-21T17:41:18+02:00  # Schedule page publish date.
draft = false

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
time_start = 2016-08-21T16:30:00+02:00
time_end = 2016-08-21T17:30:00+02:00

# Abstract and optional shortened version.
abstract = "In den letzten Jahren erfreut sich Docker und das Konzept von Containern immer grösserer Beliebtheit, insbesondere wenn man in oder für die Cloud entwickelt. Dieses Vorgehen bewirkt aber oft, dass man mitunter eine steigende Anzahl an Containern orchestrieren muss. Unterstützung beim Containermanagement bieten bereits weit verbreitet Werkzeuge wie Kubernetes, Docker Swarm oder Shipyard. Dabei ist insbesondere Kubernetes oft komplex zum Einstieg und bringt eine Vielzahl an Begriffen mit, die man erstmal lernen muss. Seit Kurzem jedoch gibt es einen Newcomer in dem Feld, Rancher, der sich immer wachsender Beliebtheit erfreut. Rancher ermöglicht einen schnellen und einfachen Start einer Multi-Agent Umgebung, da es kompatibel zu den Standard Docker Konfigurationen (docker-compose.yml) ist. In diesem Talk wird es neben einer Einführung in Rancher auch Erfahrungsberichte aus dem produktiven Einsatz von Rancher geben."
abstract_short = ""

# Name of event and optional event URL.
event = "FrOSCon 2016"
event_url = "https://programm.froscon.de/2016/events/1786.html"

# Location of event.
location = "Sankt Augustin"

# Is this a selected talk? (true/false)
selected = false

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
#   E.g. `projects = ["deep-learning"]` references `content/project/deep-learning.md`.
projects = []

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Does the content use math formatting?
math = false

# Does the content use source code highlighting?
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++



Dieser Talk besteht aus drei Teilen, anfangs wird kurz Docker erklärt und eine Einführung in Rancher gegeben, mit einer Übersicht über den aktuellen Feature-Stand und die aktuellen Entwicklungen. Dann berichten wir von unseren Erfahrungen bei der Viaboxx GmbH mit Rancher und am Ende zeigen wir in einer kurzen Demo, wie man Docker Swarm oder Kubernetes in Rancher einbinden kann. 
Rancher ist ein Docker Clustermanagement Werkzeug, das im März 2016 in der stabilen Version 1.0 erschienen ist. Bis dato wurde sowohl am Tool selber, aber auch auf Seiten der Community eine rasante Entwicklung an den Tag gelegt, so dass es regelmäßige Releases und eine rege Beteiligung auf Github gibt. Mit Rancher ist es möglich schnell mit seinen existierenden docker-compose Konfigurationen zu starten. Selbst eine verteilte Multi-Agent Umgebung aufzubauen stellt keine große Herausforderung dar. Diese kann entweder aus Rancher Agents bestehen oder man kann seine existierenden Kubernetes und Docker Swarm Agents einfach in Rancher einbinden und weiterpflegen. Das Betreiben und Integrieren von Agents auf den Plattformen der gängigen Cloud Providern (AWS, Azure, DigitalOcean, uvm.) ist bereits ein Built-in Feature und ermöglicht jederzeit die nötige Flexibilität und Skalierbarkeit, die man in seiner privaten Container Cloud erwartet, falls der Arbeitsspeicher mal wieder knapp wird. Dabei gibt es, neben der Möglichkeit Rancher über die Kommandozeile zu steuern, sowohl eine grafische Oberfläche als auch eine vollumfängliche REST-API, womit nicht nur eine einfache Nutzung sondern auch die Möglichkeit der Integration von Rancher in eine bestehende Infrastruktur gegeben ist. Mit dem Katalog Feature von Rancher ist es dabei auch möglich bereits vorhandene Rezepte von Docker Containern einzubinden und den Katalog um eigene unternehmensspezifische Softwarestacks zu erweitern. 
In der Viaboxx GmbH haben wir Rancher seit Anfang 2016 in Verwendung, dabei haben wir unterschiedliche Projekte, die vorher mit Docker im manuell gepflegten Serverbetrieb liefen, auf die Umgebung migriert und auch Continuous Deployment aus Jenkins in Rancher eingerichtet. Durch die Verwendung von Rancher ist es jetzt auch den Entwicklern möglich über die CLI-Tools von Rancher lokal die laufende Software zu warten und neue Versionen zu deployen. Dabei haben sich auch einige Aspekte von Rancher als Stärken, aber auch ein paar Einstiegsprobleme herausgestellt, die wir gerne als unsere Erfahrungen an andere weitergeben möchten.