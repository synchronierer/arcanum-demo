# Geführtes Handbuch für die öffentliche Arcanum-DEMO

**DEMO:** [https://arcanum-demo.dynv6.net](https://arcanum-demo.dynv6.net)  
**Zugangsdaten:** [öffentliche Zugangsdaten-PDF](../Arcanum_DEMO_Zugangsdaten.pdf)

Dieses Handbuch beschreibt die am 04.10.2026 geprüfte DEMO. Es verwendet synthetische Daten (frei erfundene Testdaten). Ein Laptop ist für den ersten Rundgang am übersichtlichsten, aber nicht erforderlich. Alle Abläufe sind auch auf Tablet und Smartphone und ohne Betriebssystem-spezifische Schritte beschrieben.

## 1. Schnellstart

**Rollen:** Administration verwaltet Schuljahre, Klassen, Fächer und Systemeinstellungen. Lehrkräfte sehen Lerninhalte, Schülerfortschritt, Gelingensnachweise (Nachweise eines erreichten Lernstands), den Tutorenbereich und Anwesenheit. Schüler sehen den eigenen Lernweg, Fächer, Etappen (Abschnitte eines Lernwegs), Aufgaben, Münzen und Noten.

1. Öffne die DEMO-Adresse.
2. Suche in der PDF ein Konto der gewünschten Rolle. Passwörter stehen ausschließlich dort.
3. Melde dich an und prüfe das passende Dashboard.
4. Nutze zum Verlassen „Abmelden“ oder „Ausloggen“.

Die DEMO ist gemeinsam: Gespeicherte Zuordnungen, Lernstände und Anwesenheit können für andere sichtbar sein. Für den ersten Rundgang nur Seiten, Filter und Vorschauen verwenden.

## 2. Schülerbereich

**Konto:** Schüler. **Start:** Anmeldung öffnet das Schüler-Dashboard.

1. Prüfe „Münzen & Noten“ sowie die Kacheln „OFFEN“, „AKTUELL“, „BESTANDEN“ und „GESPERRT“.
2. Öffne „OFFEN – Etappen – Anzeigen und beginnen“.
3. Wähle Fach, Thema (inhaltlicher Lernbereich), Etappe und Aufgabe.
4. Lies die Aufgabe und kehre mit der vorhandenen Navigation zurück.
5. Prüfe „BESTANDEN“ und „GESPERRT“, falls Inhalte vorhanden sind.

Für 5a–5d gibt es je fünf synthetische Schüler. Sie haben Religion/Ethik als individuelles Fach; in Jahrgang 5 gibt es keine WPF-Zuordnung. Jahrgang 6 behält seine vorhandenen WPF-/Religion-Ethik-Zuordnungen. Flexible Lerninhalte (zusätzliche Lernwege) und individuelle Fächer nur beschreiben, wenn sie im Konto sichtbar sind.

Die Kacheln „Partner“ und „Gelingensnachweis“ wurden im geprüften Schülerkonto als „inaktiv“ angezeigt. Partnersuche und Bereitschaft für einen Gelingensnachweis sind deshalb kein bestätigtes DEMO-Szenario.

## 3. Lehrkräftebereich

**Konto:** Lehrkraft. **Start:** Anmeldung öffnet das „Teacher Cockpit“.

Die geprüften Menüs sind „Übersicht“, „Themen & Etappen“, „Schülerfortschritt“, „Gelingensnachweise“, „Tutorenbereich“ und „Anwesenheit“.

1. In „Themen & Etappen“ verfügbare Inhalte und freigegebene Etappen ansehen.
2. In „Schülerfortschritt“ nur angebotene Schüler auswählen.
3. In „Gelingensnachweise“ die schulweite Tabelle öffnen, filtern und sortieren. Sie zeigt Vorname, Nachname, Klasse, Etappe und Eintrag, soweit passende Einträge existieren.
4. „Anwesenheit“ für die schulweite Übersicht öffnen.

Die Übersicht ist zum Prüfen gedacht und zeigt keine Passwörter oder privaten Kontodaten. Bearbeitungsrechte hängen von den vorhandenen Zuordnungen ab.

## 4. Tutoransicht

Die Tutoransicht (Ansicht für Klassenbetreuende) ist keine eigene Kontoart, sondern ein Bereich eines zugeordneten Lehrkraftkontos.

1. Mit der zugeordneten Lehrkraft anmelden.
2. „Tutorenbereich“ öffnen.
3. 5a, 5b, 5c oder 5d auswählen.
4. Prüfen, dass genau die fünf Schüler dieser Klasse erscheinen.

Alle vier Klassen wurden so geprüft. Die Ansicht ist gemeinsamer Datenzugriff; beim Rundgang nichts speichern.

## 5. Administrationsbereich

**Konto:** Administration. **Start:** Anmeldung öffnet das „Admin-Dashboard“.

Das gemeinsame Menü lautet „Übersicht“, „Schuldaten“, „Schuljahr & Zuordnungen“, „Zentrales Curriculum“, „Anwesenheit“, „Rechte“ und „System“.

### Schuljahr und Zuordnungen

„Schuljahr & Zuordnungen“ zeigt die geprüfte Reihenfolge:

1. „1. Schuljahr/Halbjahr“
2. „2. Jahrgang“
3. „3. Tutorien“
4. „4. REGULAR-Matrix“ (verbindliche Fächer je Klasse)
5. „5. Individuelle Lehrkräfte“
6. „6. Schülerzuordnung“

HJ1 2026/27 ist das aktive Halbjahr (aktuell gültiger Schulzeitraum). „Ausgewähltes Halbjahr aktivieren“ ändert den gemeinsamen Zustand und ist nur für geplante Tests zu verwenden.

### Curriculum und Schuldaten

- „Zentrales Curriculum“ zeigt zentrale Themen und Etappen. „Vorschau prüfen“ ist lesend; „Import bestätigen“ verändert Daten.
- „Schülerverwaltung öffnen“ zeigt Schülerliste und Klassenfilter.
- „Lehrkräfte verwalten“ zeigt Konten sowie Hinzufügen und Bearbeiten.
- „Klassenverwaltung öffnen“ zeigt Klassen, Jahrgänge und Archivierung.
- „Fächerverwaltung öffnen“ zeigt Fächer, Fachart und Zuordnungsart.

Speichern, Aktivieren, Importieren, Archivieren und Löschen verändern gemeinsam sichtbare Daten.

### Anwesenheit, Rechte und System

- „Attendance“ ist die schulweite Anwesenheitsübersicht mit Datum, Standort, Status und Klassenfiltern.
- „Attendance verwalten“ verwaltet Bereiche und QR-Codes (scanbare Zugangscodes).
- „Berechtigungen und Rollen verwalten“ zeigt `teacher`, `student` und `admin`.
- „Module verwalten“ zeigt `attendance_plugin`, `results_plugin`, `plugin-loader`, `permission-manager` und `arcanum-overlay`.

Eine Web-Zurücksetzung, SOL-Planer, SOL-Schülerübersichten, Displays/Signage, ScreenTinker und WebUntis-Anbindungen sind nicht als verfügbare DEMO-Funktionen geprüft.

## 6. Anpassbarkeit

Die DEMO zeigt REGULAR-Fächer (verbindliche Fächer) je Klasse, Religion/Ethik als individuelle Zuordnung, WPF in vorhandenen Jahrgang-6-Daten, zentrale Curricula sowie flexible Lernwege, sofern sie für ein Konto freigegeben sind. Diese Beispiele sind keine Zusage für jede Schulregel.

Fachliche Rückmeldungen und Beiträge sind über das öffentliche GitHub-Repository willkommen. Ein weiterer Support-Kanal ist nicht eingerichtet.

## 7. Ausprobier-Szenarien

### A – Zentrale Etappe und Aufgabe

- **Vorbedingung/Rolle:** Schülerkonto mit sichtbarer offener Etappe.
- **Schritte:** anmelden → „OFFEN“ → „Anzeigen und beginnen“ → Fach → Etappe → Aufgabe.
- **Ergebnis:** Aufgabe öffnet sich ohne technischen Fehler.
- **Gemeinsame Änderung:** Öffnen erzeugt keine Münzen, Leistung oder Completion (gespeicherte Aufgabenerledigung).

### B – Religion/Ethik in Jahrgang 5

- **Vorbedingung/Rolle:** Schüler aus 5a–5d.
- **Schritte:** anmelden → Fächer/Lernweg öffnen → Religion/Ethik prüfen.
- **Ergebnis:** individuelles Fach sichtbar; kein WPF in diesen Beispielen.
- **Gemeinsame Änderung:** keine.

### C – Tutoransicht

- **Vorbedingung/Rolle:** zugeordnete Lehrkraft.
- **Schritte:** anmelden → „Tutorenbereich“ → 5a, 5b, 5c oder 5d.
- **Ergebnis:** genau fünf Schüler.
- **Gemeinsame Änderung:** keine.

### D – Gelingensnachweise

- **Vorbedingung/Rolle:** Lehrkraft und passende Einträge.
- **Schritte:** anmelden → „Gelingensnachweise“ → Tabelle öffnen → filtern/sortieren.
- **Ergebnis:** relevante Schüler-Etappen ohne private Kontodaten.
- **Gemeinsame Änderung:** keine.

### E – Admin-Rundgang

- **Vorbedingung/Rolle:** Administration.
- **Schritte:** „Schuljahr & Zuordnungen“, „Zentrales Curriculum“, „Attendance“, „Berechtigungen und Rollen verwalten“ und „Module verwalten“ öffnen; nur lesen und Vorschauen nutzen.
- **Ergebnis:** Seiten laden und zeigen den aktuellen Zustand.
- **Gemeinsame Änderung:** keine, solange keine Aktion bestätigt wird.

### F – Tablet und Smartphone

- **Vorbedingung/Rolle:** beliebiges mobiles Gerät und beliebige Rolle.
- **Schritte:** DEMO öffnen → anmelden → Menü öffnen → vertikal scrollen.
- **Ergebnis:** geprüfte Ansichten bleiben bedienbar; seitliches Scrollen soll nicht nötig sein.
- **Gemeinsame Änderung:** keine.

Partnersuche und Bereitschaft für einen Gelingensnachweis sind wegen „inaktiv“ nicht als PASS-Szenarien aufgenommen. Anwesenheitsbestätigung, Import, Archivierung und Rollenänderung sind keine reinen Lesetests.

## 8. Begriffe und Prüfstand

Fachbegriffe werden beim ersten Auftreten in einfachen Worten erklärt. Menü- und Schaltflächennamen entsprechen der geprüften DEMO; „Teacher Cockpit“ und „Attendance“ bleiben englische Oberflächenbegriffe.

Geprüft wurden öffentliche URL, Anmeldung für alle drei Rollen, Admin-Unterseiten, Tutoransicht 5a–5d, Lehrkraftübersicht und Schüleroberfläche. Die Prüfung war lesend; keine DEMO-Daten wurden verändert. Die vier technischen Konten und die 138 Zugangsdaten wurden nicht erneut vollständig angemeldet.
