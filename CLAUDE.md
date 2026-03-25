# CLAUDE.md — Arbeitsweise für dieses Projekt

Basierend auf Boris Cherny's Workflow-Framework.

---

## Workflow Orchestration

### 1. Plan Mode Default
- Vor JEDER nicht-trivialen Aufgabe (3+ Schritte oder inhaltliche Entscheidungen): Plan schreiben
- Wenn etwas schiefläuft: STOP — neu planen, nicht weiter hacken
- Plan Mode auch für Verifikationsschritte, nicht nur für die Umsetzung
- Spezifikationen detailliert aufschreiben, bevor mit der Arbeit begonnen wird

### 2. Subagent-Strategie
- Subagents grosszügig einsetzen, um den Haupt-Kontext sauber zu halten
- Recherche, Exploration und parallele Analysen an Subagents auslagern
- Bei komplexen Aufgaben: mehr Compute einsetzen via Subagents
- Ein Task pro Subagent — fokussierte Ausführung

### 3. Self-Improvement Loop
- Nach JEDER Korrektur durch den User: Lessons in `tasks/lessons.md` festhalten
- Regeln schreiben, die denselben Fehler in Zukunft verhindern
- Lessons konsequent iterieren bis die Fehlerrate sinkt
- Zu Beginn jeder Session: relevante Lessons reviewen

### 4. Verification Before Done
- Niemals eine Aufgabe als erledigt markieren, ohne zu beweisen, dass sie funktioniert
- Verhalten vor und nach Änderungen vergleichen
- Frage stellen: *"Würde ein Senior das so abnehmen?"*
- Tests laufen lassen, Logs prüfen, Korrektheit demonstrieren

### 5. Eleganz fordern (ausgewogen)
- Bei nicht-trivialen Änderungen: pausieren und fragen *"Gibt es einen eleganteren Weg?"*
- Wenn eine Lösung sich hacky anfühlt: elegante Lösung implementieren
- Bei einfachen, offensichtlichen Fixes: nicht over-engineeren
- Eigene Arbeit hinterfragen, bevor sie präsentiert wird

### 6. Autonomes Arbeiten
- Bei klaren Aufgaben: einfach erledigen — kein Hand-Holding nötig
- Auf Logs, Fehler und Probleme hinweisen — dann lösen
- Kein Kontext-Wechsel für den User erforderlich

---

## Task Management

1. **Plan First** — Plan in `tasks/todo.md` schreiben mit abhakbaren Items
2. **Plan verifizieren** — Vor der Umsetzung kurz einchecken
3. **Fortschritt tracken** — Items als erledigt markieren, während gearbeitet wird
4. **Änderungen erklären** — High-level Summary bei jedem Schritt
5. **Ergebnisse dokumentieren** — Review-Sektion in `tasks/todo.md` hinzufügen
6. **Lessons festhalten** — `tasks/lessons.md` nach Korrekturen aktualisieren

---

## Core Principles

- **Simplicity First** — Jede Änderung so einfach wie möglich. Minimaler Einfluss auf bestehenden Code/Content.
- **No Laziness** — Ursachen finden. Keine temporären Fixes. Senior-Standard.
- **Minimal Impact** — Nur anfassen, was nötig ist. Keine Nebeneffekte, keine neuen Probleme.

---

## Projektkontext

**Brand:** LM Dents
**Inhaber:** Pius
**Nische:** Social Media Strategie für lokale Unternehmen (Fokus: Dentalpraxen)
**Plattformen:** Instagram (Reichweite) + LinkedIn (Autorität)
**Phase:** Foundation Building — Publikum aufbauen, Vertrauen etablieren
**Sprache:** Deutsch (Content) / Englisch (technische Files)
**Branch:** `claude/dental-social-strategy-zT6aI`

**Brand Colors:**
- Schwarz: `#0A0A0A`
- Blau: `#2B5CE6`
- Weiss: `#FFFFFF`

**Aktuelle Deliverables:**
- `30-day-content-calendar.md` — Vollständiger 30-Tage-Kalender
- `posts-de.html` — 5 Posts auf Deutsch, PDF-ready mit Brand Styling
