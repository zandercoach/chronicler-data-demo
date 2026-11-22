# Chronicler demo

A small, invented chronicle for the [Chronicler engine](https://github.com/zandercoach/chronicler-engine), published at **https://chronicler.adaptive-x-ai.org**. It is part of the learning journey [Adaptive × AI](https://adaptive-x-ai.org).

The story — *Der verlorene Zehnt* and *Der Turm im Nebelmoor* — started as the engine's test fixture; this repo holds a copy, so the two can grow apart. Everything in it is invented for the purpose; wiki links point to the German Wikipedia.

## Layout

- `data/` — the chronicle as XML: `data.xml` ties the endeavors, members, stakeholders, creatures, locations and sessions together; `chronicler.xml` configures the instance (title, welcome text, copyright, wiki source, legal links, map, calendar).
- `img/` — pictures per type; a missing one falls back to `default.jpg`.
- `briefs/` — one image brief per picture, in the „zander.coach flipchart style"; the rules are in `IMAGE-STYLE.md`, a supplement of the workspace's image-style core.

## Publishing

Every push to `main` runs `.github/workflows/publish.yml`: the engine's `main` generates the chronicle, the engine's invariant tests check it, and GitHub Pages serves the result. Pull requests are generated and checked, not published.

Dates follow the chronicle's own calendar, configured in `chronicler.xml`: twelve months from Eismond to Frostmond and five Flutnächte, counted „nach der Flut“. The data writes `1.NEB 1001 n. F.`, the pages show `1. Nebelmond 1001 n. F.`
