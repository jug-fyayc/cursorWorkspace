# Workspace Beschreibung für Git

Dieser Workspace dient als zentrale Arbeitsumgebung für die Entwicklung, das Testen und die Dokumentation von Projekten, die mit Git versioniert werden. Er ist so strukturiert, dass die Zusammenarbeit im Team effizient gestaltet werden kann und eine klare Trennung von Quellcode, Konfigurationsdateien, erzeugten Artefakten und Dokumentationen gewährleistet ist.

## Struktur

- **Root-Verzeichnis:** Hier liegen zentrale Dateien wie `README.md`, `.gitignore`, `.gitmodules` sowie automatisch generierte Dateien und Skripte.
- **step-cursor-workspace:** Enthält den eigentlichen Projektcode sowie wichtige Definitions- und Regeldateien.
- **/localDocumentation/**: (Falls vorhanden) Für lokale, nicht versionierte Dokumentationen.
- **.cursor/rules/**: Enthält spezifische Regeln zu Coding-Standards, Dokumentationsprozessen, Ablageorten und Subagenten-Verhalten, um eine konsistente Entwicklung zu gewährleisten.

## Besonderheiten

- **Submodule:** Der Workspace kann über Git-Submodule erweitert werden, um Code oder Artefakte aus externen Repositories einzubinden (siehe `.gitmodules`).
- **Automatisierte Ablage:** Vom Agent oder Tooling generierte Dateien werden per Standard im Root-Verzeichnis abgelegt, sofern nichts anderes definiert ist.
- **Konventionen & Standards:** Durch definierte Regeln in `.cursor/rules/` werden Code-Qualität, Dokumentation und Ablageorte sichergestellt.

## Zusammenarbeit

- Änderungen sollten stets über Branches und Pull Requests erfolgen, um Qualität und Nachvollziehbarkeit zu gewährleisten.
- Die Benutzung von `.gitignore` stellt sicher, dass keine temporären oder sensiblen Dateien ins Repository gelangen.

---

> Diese README gibt einen Überblick über den Aufbau und Arbeitsweise des Workspaces im Kontext der Versionskontrolle mit Git. Für spezifische Coding-Guidelines und Ablageorte siehe bitte die Dokumentationen im Ordner `.cursor/rules/`.
