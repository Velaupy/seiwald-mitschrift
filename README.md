# seiwald-mitschrift

Das ist die README.md-Datei. MD steht für Markdown. Markdown ist eine heutzutage weit verbreitete Auszeichnungssprache. (*Markup Language*, [Wikipedia](https://de.wikipedia.org/wiki/Auszeichnungssprache)).

Weiter bekannte Auszeichnungssprachen sind:

- Hypertext Markup Language (HTML)
- Extensible Markup Language (XML)
- Yet Another Markup Language (YAML, YML)

# Installation von Node.js

Javascript läuft unter normalen Umständen in einer Browser-Sandbox (nur im Browser).
Seit ca. 2010 gibt es eine Laufzeitumgebung (*Runtime Environment*) für JS, damit man auch serverseitig JS programmieren kann: [Node.js](https://nodejs.org)

# Installation von pnpm

Der standardmäßige *Package Manager* für Node.js ist `npm` (*Node Package Manager*). Eine etwas modernere und inzwischen beliebtere Variante ist [`pnpm`](https://pnpm.io)

# Installation von Strapi

Installation mit dem Skript `pnpm create strapi`. Daraufhin führt das CLI durch die Installation. Falls bei der Installation sogenannte "build scripts" nicht ausgeführt werden kann, schlägt die CLI die Fehlerbehandlung selbstständig vor:

1. Wechsel in das Installationsverzeichnis (z.B. mit `cd my-strapi-projekt`)
2. Neuerlicher Versuch der Installation mit `pnpm install`. Dieser Scheitert in der Regel - die Build-Skripte müssen mit `pnpm approve-build` manuell freigegeben werden.

---

# Historische Entwicklung von WebDev

Webdevelopment hat im Laufe der letzten rund 35 Jahre einige Evolutionsstufen durchlaufen:

1. Statische Website (HTML, CSS, ggf. JavaScript) - initiale Phase des Webdevelopments, bei der Inhalte fest im HTML-Code verankert sind. Dominant in den 1990er-Jahren.
2. Dynamische Website (mit serverseitiger Programmiersprache - PHP, Python, NodeJS - und Datenbankanbindung). Dominant in den 2000er-Jahren.
3. *Single-Page Application* (SPA) - mit JavaScript-Frameworks erstellte "Webapps", die ähnliche Funktionen wie klassische Desktop-Anwendungen bzw. Handy-Apps bieten. Dominant in den 2010er-Jahren. Um Handy-Apps möglicht nahe zu kommen, wurde der *Progressive Web App* (PWA)-Standard entwickelt. Damit können Webapps offline funktionieren, Push-Benachrichtigungen senden lassen, und auf bestimmte native Funktionen des Geräts zugreifen. Es gibt drei Voraussetzungen, die eine Webapp erfüllen muss, um als PWA zu gelten:
	1. Die Webapp muss über ein Web-App-Manifest verfügen (`manifest.json`), das grundlegende Informationen über die App enthält (Name, Icons, Start-URL, etc.).
	2. Die Webapp muss einen Service Worker implementieren, der das Caching von Ressourcen und die Offline-Funktionalität ermöglicht. Ein Service Worker ist eine JavaScript-Datei, die im Hintergrund des Browers läuft - selbst wenn der Browser geschlossen ist.
	3. Die Webapp muss über HTTPS bereitgestellt werden, um die Sicherheit und Integrität der Anwendung zu gewährleisten.

Frontend-Frameworks wenden folgende Architekturprinzipien an, um eine möglichst gute *User Experience* (UX) zu erreichen:

- **Komponenten** - Komponenten sind die wiederverwendbaren "Lego"-Bausteine einer Webapp. Sie kapseln HTML, CSS und JavaScript in einer einzigen Einheit, die unabhängig von anderen Komponenten entwickelt, getestet und gewartet werden kann.
- **Deklarative Programmierung** - der JavaScript- und Template(HTML)-Code beschreiben, wie die Benutzeroberfläche aussehen soll, anstatt die einzelnen Schritte zur Erstellung der Benutzeroberfläche zu definieren. Das Framework kümmert sich um die Umsetzung. Dabei kommt **Reaktivität** (*reactivity*) ins Spiel: Wenn sich der Zustand der Anwendung ändert, aktualisiert das Framework automatisch die Benutzeroberfläche, um den neuen Zustand widerzuspiegeln. Wenn die Aktualisierung auch in die andere Richtung funktioniert (d.h. wenn sich die Benutzeroberfläche ändert, weil der Benutzer mit ihr interagiert, und der Zustand (*state*) der Anwendung entsprechend aktualisiert wird), spricht man von bidirektionaler Datenbindung (*two-way data binding*). Logikbausteine (Schleifen zur Darstellung von Listen und Bedingungen für das konditionale Ein- und Ausblenden von UI-Elementen) werden in den Templates (HTML) der Komponenten definiert. Die Templates werden vom Framework in die eigentliche Benutzeroberfläche übersetzt. Komponenten können auch andere Komponente enthalten (verschachelt werden), wodurch eine hierarchische Struktur entsteht. Die Kommunikation zwischen Komponenten erfolgt über **Props** (Eigenschaften) und **Events** (Ereignisse). Props sind Daten, die von einer übergeordneten Komponente an eine untergeordnete Komponente weitergegeben werden. Events sind Benachrichtigungen, die von einer untergeordneten Komponente an eine übergeordnete Komponente gesendet werden, um auf Benutzerinteraktionen oder andere Ereignisse zu reagieren.

# VibeCoding / AgenticEngineering mit VS-Code und GitHub Copilot

VibeCoding passiert in VS-Code in erster Linie über die neu eingeführte Agent View. Dort können alle Anpassungen des "_Coding Harness_" vorgenommen werden. Wir können unseren _Harness_ mit verschiedenen Methoden anpassen: