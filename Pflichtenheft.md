### Einleitung

#### Zweck
Das Pflichtenheft beschreibt die Anforderungen und Spezifikationen für die Entwicklung einer maßgeschneiderten QA-Management-Software, die den gesamten Testprozess verwaltet und optimiert.

#### Zielgruppe
- **Entwicklerteam:** Umsetzung der Softwareanforderungen.
- **QA-Team:** Nutzung der Software zur Testverwaltung.
- **Administratoren:** Verwaltung der Benutzer und Projekte.

### Systemübersicht

Die QA-Management-Software ermöglicht die Verwaltung von Projekten, Testfällen, Testplänen und Testläufen. Benutzer können Testfälle erstellen, zuweisen, durchführen und deren Status verfolgen. Die Software bietet Berichterstellungsfunktionen und ermöglicht die Dokumentation von Testergebnissen.

### Detaillierte Anforderungen

#### Funktionale Anforderungen

##### Benutzer- und Rollenverwaltung
- **Registrierung und Anmeldung:**
  - Benutzer können sich registrieren und anmelden.
  - Registrierung erfordert Name, E-Mail, Passwort und Rolle.
- **Rollenbasierte Zugriffskontrolle:**
  - Admins haben vollen Zugriff, Tester eingeschränkten Zugriff.
- **Passwort-Management:**
  - Möglichkeit zum Ändern und Zurücksetzen von Passwörtern.

##### Projektverwaltung
- **Erstellung, Bearbeitung und Löschung von Projekten:**
  - Admins können Projekte verwalten.
- **Zugehörige Module:**
  - Projekte können in Module unterteilt werden.

##### Testfallverwaltung
- **Testfälle erstellen, bearbeiten und löschen:**
  - Tester/Admins können Testfälle verwalten.
- **Attribute eines Testfalls:**
  - Alle erforderlichen Felder wie in den Anforderungen beschrieben.
- **Wiederverwendbarkeit und Organisation:**
  - Testfälle können in verschiedenen Testläufen verwendet werden.

##### Testpläne und Testläufe
- **Testpläne erstellen, bearbeiten und löschen:**
  - Admins können Testpläne erstellen.
- **Testläufe erstellen, bearbeiten und löschen:**
  - Testläufe innerhalb von Testplänen verwalten.
- **Zuweisung von Testern und Testfällen:**
  - Testfälle zu Testläufen und Testern zuweisen.

##### Statusverfolgung und Fortschrittsanzeige
- **Statuswerte verwalten:**
  - Nicht gestartet, In Bearbeitung, Abgeschlossen, Fehlgeschlagen, Blockiert.
- **Dashboard:**
  - Übersicht über den Testfortschritt pro Projekt und Testlauf.
  - Visualisierung durch Diagramme und farbliche Markierungen.

##### Dokumentation und Anhänge
- **Separate Kommentare:**
  - Benutzer können Kommentare getrennt von den Hauptdaten hinzufügen, um Diskussionen und Feedback klar zu strukturieren.
- **Direktes Speichern von Screenshots:**
  - Benutzer können Screenshots direkt in den Testfällen speichern, um visuelle Hinweise und Fehlerdokument
