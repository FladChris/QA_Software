# QA-Management-System

## Beschreibung

Entwicklung einer maßgeschneiderten QA-Management-Software zur effizienten Verwaltung, Durchführung und Dokumentation von Testfällen. Die Anwendung bietet Benutzer- und Rollenverwaltung, Projektmanagement, Testfallverwaltung mit getrennten Kommentaren und direktem Speichern von Screenshots sowie zukünftige GitLab-Integration.

## Projektübersicht

Dieses Projekt zielt darauf ab, eine benutzerdefinierte QA-Management-Software zu entwickeln, die speziell auf die Anforderungen unseres Unternehmens zugeschnitten ist. Die Software soll den gesamten Qualitätssicherungsprozess effizienter, strukturierter und nachvollziehbarer gestalten, indem sie zentrale Funktionen zur Verwaltung, Durchführung und Dokumentation von Testfällen bereitstellt.

## Features

- **Benutzer- und Rollenverwaltung**
  - Verwaltung von Benutzern mit unterschiedlichen Rollen (Administrator, Tester, Entwickler)
  - Registrierung und Anmeldung (ggf. durch SSO google)

- **Projektverwaltung**
  - Erstellung, Bearbeitung und Verwaltung von Projekten

- **Testfallverwaltung**
  - Erstellung, Bearbeitung und Organisation von Testfällen
  - Verwaltung von Testfall-Attributen (Titel, Beschreibung, Status, zugewiesener Tester, Testsystem, Testgrund, Voraussetzungen, Use Cases, Testschritte, erwartetes und tatsächliches Ergebnis)
  - Getrennte Kommentarfunktion für klare Diskussionen
  - Direkte Speicherung von Screenshots
  - Verknüpfung von GitHub-Links für relevante Repositories oder Bug-Tickets

- **Testpläne und Testläufe**
  - Planung und Durchführung von Testläufen innerhalb definierter Testpläne
  - Statusaktualisierung während der Testdurchführung

- **Statusverfolgung und Fortschrittsanzeige**
  - Verfolgung des Teststatus (Nicht gestartet, In Bearbeitung, Abgeschlossen, Fehlgeschlagen, Blockiert)
  - Dashboard mit Echtzeit-Übersicht über den Testfortschritt

- **Dokumentation und Anhänge**
  - Hinzufügen von Kommentaren und Notizen zu Testfällen
  - Hochladen und Verwalten von Anhängen (Screenshots, Dokumente)

- **Berichterstellung und Export**
  - Generierung von Berichten über den Testfortschritt und die Testergebnisse
  - Export von Berichten als PDF oder CSV

## Geplante Technologien

- **Backend:** Python mit Flask
- **Frontend:** HTML5, CSS3 (Tailwind CSS), JavaScript (optional für zusätzliche Interaktivität)
- **Datenbank:** SQLite
- **Versionierung:** GitLab ggf. später wechsel auf GitLab
- **Entwicklungsumgebung:** Visual Studio Code (VSC)

## Installation

### Voraussetzungen

- Python 3.8+
- SQLite
- Git

### Schritte

1. **Repository klonen:**
    ```bash
    git clone https://gitlab.com/dein-benutzername/qa-management-system.git
    cd qa-management-system
    ```

2. **Virtuelle Umgebung erstellen und aktivieren:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # Für Linux/Mac
    # .\venv\Scripts\activate  # Für Windows
    ```

3. **Abhängigkeiten installieren:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Umgebungsvariablen konfigurieren:**
    Erstelle eine `.env` Datei im Projektstammverzeichnis mit folgendem Inhalt:
    ```
    FLASK_APP=app.py
    FLASK_ENV=development
    SECRET_KEY=dein_geheimnis
    SQLALCHEMY_DATABASE_URI=sqlite:///qa.db  # Oder deine PostgreSQL-URI
    JWT_SECRET_KEY=dein_jwt_geheimnis
    ```

5. **Datenbank initialisieren:**
    ```bash
    flask db init
    flask db migrate -m "Initial migration."
    flask db upgrade
    ```

6. **Server starten:**
    ```bash
    flask run
    ```

7. **Frontend einrichten:**
    Öffne `app/templates/` und bearbeite die HTML-Dateien nach Bedarf. Tailwind CSS ist bereits integriert via CDN.

    - Füge getrennte Kommentare und speichere Screenshots direkt in den Testfällen.

6. **Berichte generieren und exportieren:**
    - Erstelle Berichte über den Testfortschritt und exportiere sie bei Bedarf.
