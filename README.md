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
3. *Single-Page Application* (SPA) - mit JavaScript-Frameworks erstellte "Webapps", die ähnliche Funktionen wie klassische Desktop-Anwendungen bzw. Handy-Apps bieten. Dominant in den 2010er-Jahren.

# VibeCoding / AgenticEngineering mit VS-Code und GitHub Copilot

VibeCoding passiert in VS-Code in erster Linie über die neu eingeführte Agent View. Dort können alle Anpassungen des "_Coding Harness_" vorgenommen werden. Wir können unseren _Harness_ mit verschiedenen Methoden anpassen: