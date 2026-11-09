# Projekt-Karte

Dieses Projekt läuft über die **Software Factory**.

## Ablauf
1. `/init`: einmal zu Beginn. Liest `docs/briefing.md`, legt Vision (`docs/PRD.md`), Stack (`docs/stack.md`), Design (`docs/design-system.md`) und Feature-Karte (`features/INDEX.md`) fest und richtet das Projekt-Grundgerüst ein.
2. `/write-spec PROJ-X`: Spec für ein Feature im Interview erarbeiten → `features/PROJ-X-name/spec.md`. Die Spec ist der Vertrag.
3. `/to-factory PROJ-X`: an die Factory übergeben. Die Factory baut, testet und öffnet einen Pull Request.
4. Pull Request prüfen (inkl. Vorschau-Link) und mergen.

## Wo was liegt
- `docs/briefing.md`: Ausgangslage
- `docs/PRD.md`: Vision und Ziele
- `docs/stack.md`: Technik-Entscheidungen und Konventionen (verbindlich für die Factory)
- `docs/design-system.md`: Gestaltung
- `features/`: Feature-Karte und pro Feature `spec.md` (du), `design.md` + `qa-report.md` (Factory)
- `.factory/setup.json`: wie installiert, gestartet und geprüft wird
- `.factory/Dockerfile` (optional): zusätzliche Werkzeuge für die Factory, falls der Stack nicht auf Node läuft

## Regeln
- Erst die Spec, dann die Umsetzung. Kein Feature ohne `spec.md`.
- Commits: `typ(PROJ-X): Beschreibung`
