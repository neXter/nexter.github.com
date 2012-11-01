---
comments: true
date: 2006-02-23 12:00:40
layout: post
slug: verbesserte-grafikengine-im-kommen
title: Verbesserte Grafikengine im Kommen
wordpress_id: 1112
categories:
- News
- Tipps
tags:
- grafik
- News
- technik
- world-of-warcraft
---

Wahrscheinlich in Hinsicht auf die angekündigten OpenPvP Ergänzungen und dadurch häufigere Ansammlung großer Spielermengen an einer Position im Spiel arbeitet Blizzard zur zeit an einer verbesserten Grafikengine, die die Darstellung vieler Spieler auf einmal verbessert, teilweise drastisch. Wie der TechSupport im off. Forum schreibt ist diese Änderung bereits jetzt testbar, durch einen einfachen Eingriff in die WoW Dateien. Da dieser Vorschlag von off. Seite kommt braucht man auch keinen Ban zu fürchten.



> Mit Patch 1.9.3 wurde Programmcode implementiert für den es bislang noch keine Option im Menü gibt und der im Moment noch als experimentell einzustufen ist, da er von uns noch nicht hundertprozentig getestet wurde. Diese Option kann sowohl auf Windows- als auch auf Macintosh-Clients gesetzt werden.

Der neue Programmcode nutzt eine Technik für die Darstellung von Szenen in denen viele Spielfiguren auf einmal gezeichnet werden müssen. Technisch gesprochen versuchen wir zu verhindern, dass der Vertex-Shader bei der Verarbeitung eines einzelnen Frames zu oft umprogrammiert werden muss. Bei Systemen, die über keinen Vertex-Shader verfügen oder bei denen die Shader deaktiviert sind, wird diese Änderung keinerlei Effekt haben.

Bei internen Tests konnten wir zu Zeiten, zu denen Ironforge gerammelt voll war eine Zunahme der Bildrate von bis zu 30% feststellen – abhängig vom eingesetzten Betriebssystem, der CPU und GPU und dem Inhalt der Szene. Bestimmte GPUs profitieren hierbei weitaus mehr von der Veränderung als andere.

Die Variable, die wir eingefügt haben lautet M2Faster, welche ihr testen könnt, indem ihr die Datei config.wtf Datei editiert und an deren Ende einfach die folgende Zeile einfügt:

SET M2Faster "1"

Startet das Spiel danach erneut. Um den Parameter zu deaktivieren löscht diese Zeile einfach wieder oder setzt statt der “1“ eine “0“ ein. In Version 1.9.3 ist der Parameter standardmäßig deaktiviert.

(M2 ist der interne Name für das von World of Warcraft benutzte Modeling-/Animationssystem)

Ihr werdet keinerlei Veränderungen im Freien oder in wenig bevölkerten Gebäuden/Räumen sehen. Möglicherweise nicht einmal in vollen Gebäuden, wenn Eure CPU ohnehin schnell genug ist. Diese Änderung dient vor allem der Entlastung der CPU und Treiber auf schwächeren Systemen, die aber über eine vertex-shader-fähige GPU verfügen. 



Quelle: [Off. Technik Forum (DE)](http://forums-de.wow-europe.com/thread.aspx?fn=wow-tech-support-de&t=192287&p=1&tmp=1#post192287)

[Robert](http://www.robert-guenther.com/blog/) hat dies grad getestet, sein Statement: 

> "Hmm, also IF war grad nich so voll. Aber es hat schon recht fix geladen. Auf jeden fall schneller als vorher, vor allem hat er instant alle Figuren dargestellt und nicht erst nach einer Weile." "Und wie war dein Lag beim Drehen und Laufen in IF?" "Null."
