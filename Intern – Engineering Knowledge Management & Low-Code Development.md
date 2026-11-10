Bosch (ME-SN Engineering) | [Start – 2026]

# Summary
Entwicklung einer internen Knowledge-Management-Lösung für Engineering-Work-Packages auf der Microsoft Power Platform, mit Power Apps, Power Automate und SharePoint. Dazu kamen eigene Git-basierte ALM-Prozesse und Experimente mit KI-Assistenten (Copilot).

# Application Development (Power Apps)

- Entwickelte und erweiterte eine Canvas App mit mehreren Screens (Home, Work-Package-Erstellung, Suche, Admin) für die Verwaltung von Engineering-Work-Packages.
- Implementierte Formulare, Galerien, Single- und Multi-Select-ComboBoxes, Validierung und bedingte UI-Logik in Power Fx.
- Baute Mehrkriterien-Filter- und Suchfunktionen auf Metadaten-Basis mit dynamischen Ergebnisansichten. Dabei wog ich Flexibilität, Performance und Usability ab.
# Workflow Automation (Power Automate)

- Automatisierte mehrstufige Geschäftsprozesse: Anlegen und Aktualisieren von Work Packages, Erzeugen standardisierter Ordnerstrukturen (Input / Working / Review / Released Result) und Verarbeiten von Metadaten.
- Band die Flows an die App an (Parameterübergabe, Rückgabe von Ergebnissen) und passte sie an neue Anforderungen an.
- Analysierte fehlerhafte Flow-Läufe anhand von Run-History und Zwischenwerten.
# SharePoint & Berechtigungskonzept

- Nutzte SharePoint-Listen und Dokumentbibliotheken als Backend und integrierte sie mit Power Apps und Power Automate.
- Entwarf und dokumentierte ein Berechtigungskonzept: Normale Nutzer können Hauptordner nicht manuell anlegen, sondern nur kontrolliert über die App. Innerhalb eines Work Packages können sie Dateien bearbeiten.
- Setzte dies um mit Vererbungssteuerung, Rollen/Gruppen und automatisierter Rechtevergabe über Flows und SharePoint-HTTP-/REST-Aufrufe.
# Datenintegration

- Verarbeitete und transformierte JSON-Daten und mappte externe Datenstrukturen auf SharePoint-Datenmodelle.
- Entwarf Naming-Conventions und eindeutige Identifier, behandelte fehlende Werte und verhinderte Duplikate (Create-vs-Update-Logik).
# AI & Copilot

- Evaluierte und prototypte interne KI-Assistenten mit Microsoft 365 Copilot Agent Builder und Copilot Studio.
- Schrieb Agent-Instruktionen und Skill-Definitionen, z. B. Suche und Zusammenfassung von Work Packages oder Filtern nach Domain, Status und Owner.
- Untersuchte Grounding auf Organisationswissen und die Anbindung über Microsoft Teams.
# ALM, Versionskontrolle & Automatisierung

- Richtete Versionskontrolle für Low-Code-Lösungen ein mit Git, GitHub Enterprise und Power Platform CLI (pac). Exportierte Solutions in lesbaren Quellcode zur Sicherung und Nachvollziehbarkeit.
- Schrieb PowerShell-Skripte, die Export, Backup und Repository-Synchronisierung wiederholbar machen.
- Erarbeitete einen Branching- und Merge-Ansatz für künftige Weiterentwicklung.
- Erstellte Dokumentation in Markdown, die unabhängig vom Entwickler-Rechner nutzbar ist.
**Technologien**
Power Apps, Power Fx, Power Automate, SharePoint, Microsoft 365, Copilot Studio, Agent Builder, Teams, Power Platform CLI, Git, GitHub Enterprise, VS Code, PowerShell, JSON, Markdown

# Kurzversion (für Lebenslauf mit wenig Platz)
- Entwickelte eine Power-Apps-/Power-Automate-Lösung mit SharePoint-Backend zur Verwaltung und Suche von Engineering-Work-Packages.
- Entwarf ein rollenbasiertes SharePoint-Berechtigungskonzept mit automatisierter Ordner- und Rechtevergabe.
- Etablierte einen Git-/pac-/PowerShell-basierten ALM-Prozess für Low-Code-Lösungen, einschließlich Backup und Dokumentation.
- Prototypte KI-Assistenten mit Copilot Studio und Agent Builder auf Basis von Organisationswissen.
# Empfehlungen

Ergänze, wenn möglich, Zahlen. Beispiele: Anzahl der Nutzer, Zeitersparnis pro Work Package, Anzahl der Flows oder Screens.
Passe die Schwerpunkte an die Stelle an. Für Software-Rollen betone ALM, Git und PowerShell. Für Prozess- oder Digitalisierungsrollen betone Automatisierung und Berechtigungskonzept. Für KI-Rollen betone den Copilot-Teil.
Sag mir die Sprache (Deutsch oder Englisch) und die Zielstelle. Dann schreibe ich eine passende Fassung.