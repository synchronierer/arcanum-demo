# Interne Screenshot-Abnahme

Stand: 17.10.2026. Die vorhandenen Aufnahmen stammen aus frischen
Browser-Sitzung gegen die laufende DEMO. Die erste Prüfung erfolgte unmittelbar
im Browser nach der Navigation; die zweite Prüfung erfolgte durch erneutes
visuelles Öffnen der gespeicherten PNGs. Für die zweite Sichtprüfung wurden
alle 17 Dateien einzeln in einer Kontaktansicht erneut geöffnet und auf
Beschriftung, Zustand, Ausschnitt und Überlauf verglichen.

## Abnahmeergebnis

| Rolle | PNGs | Browserprüfung | PNG-Sichtprüfung | Ersetzt | Nicht akzeptiert |
|---|---:|---|---|---:|---:|
| Schüler | 8 | PASS für gezeigte Zustände; `/results` für drei Konten HTTP 200 | PASS für die aktualisierten Anton-/Berta-Bilder | 6 | 0 |
| Lehrkraft | 8 | PASS für Cockpit/Fortschritt/Detail; Verlauf FAILED | PASS | 0 | 0 |
| Administration | 10 | PASS für Lesesichten; Rollen-/Moduldetails NI-SA | PASS | 0 | 0 |
| Gesamt | 25 | nicht pauschal PASS: einzelne Funktionen FAILED/NI-SA | PASS | 0 | 0 |

Die Bilder zeigen ausschließlich veröffentlichte synthetische DEMO-Namen,
keine ausgefüllten Passwortfelder, Sitzungs- oder Zugriffstokens, echten
E-Mail-Adressen oder Freitexte. Die `/results`-Fehleransicht wurde nicht als
gefüllte Schatzkammer veröffentlicht. Leere Etappenstände werden nur als
Anton-Apfel-Livezustand beschrieben, nicht als allgemeiner Systemzustand.

## Zuordnung

### Schüler

- `00-anmeldung-live.png`: `/login`, 1440 px; leere Anmeldemaske ohne
  eingetragenes Passwort.
- `01-dashboard-live.png`: Anton Apfel, `/dashboard`, 1440 px; Profil,
  Notengrenzen, 6 Münzen und aktueller Mathe-Fortschritt sichtbar.
- `02-avatar-dialog-live.png`: Anton Apfel, geöffneter Avatar-Dialog;
  Auswahlfunktion sichtbar, keine Auswahl gespeichert.
- `03-berta-dashboard-live.png`: Berta Banane, aktuelles Mathematikangebot
  und synthetischer Kontostand.
- `04-berta-mathematik-live.png`: Mathematik mit bestätigter Etappe,
  Fehlversuch und fachlicher Notengrenze.
- `05-berta-wpf-live.png`: WPF-Angebot ohne neue Leistung im Semester-Neuaufbau.
- `06-berta-schatzkammer-live.png`: aktuelle Ergebnisse mit einer bestätigten
  Mathe-Leistung und 1 Münze.
- `07-anton-schatzkammer-final.png`: Anton Apfel, `/results`, 6 Gesamtmünzen;
  der variable Eintrag „3 von 5 Münzen“ ist im Mathe-Erfolgslogbuch sichtbar.

### Lehrkraft

- `01-cockpit-live.png`: Dora Dinkel, Übersicht mit 6d und zwei Fächern.
- `02-themen-etappen-live.png`: Kontext 6d Gesellschaftslehre, Budget,
  zentrale/flexible Themen und Freigabestatus.
- `03-schuelerfortschritt-live.png`: Kontext 6d Gesellschaftslehre,
  gefüllte Schüler- und Signal-Tabelle.
- `04-gelingensnachweise-live.png`: gefüllte GN-/Fehlversuchsübersicht mit
  Lesefiltern.
- `05-tutorbereich-live.png`: Tutor-Klasse 6d, 25 Schüler, Fachmünzen und
  Noten.
- `06-anwesenheit-live.png`: Anwesenheitsfilter und Momentaufnahme mit 222
  Schülern.
- `07-schueler-detail-live.png`: tatsächlich geöffnete Detailansicht für
  Anton Banane mit Etappen, Bewertungen und Verdienstspalten.
- `08-tutorverlauf-live.png`: Tutorübersicht mit Verlaufsschaltflächen; der
  Klick auf Verlauf öffnete im Zweitlauf keine separate Ansicht und wird nicht
  als Verlaufsscreenshot ausgegeben.

### Administration

- `01-dashboard-live.png`: Ada Ananas, aktives Halbjahr und Kennzahlen.
- `02-schuelerverwaltung-live.png`: Schülerimport, Export, Filter und Liste.
- `03-lehrkraefte-live.png`: Lehrkraftformular, CSV und Liste.
- `04-klassen-live.png`: Klassenformular und Klassenübersicht.
- `05-faecher-live.png`: Fachtypen und Aktivierung je Jahrgang.
- `06-attendance-admin-live.png`: QR-Bereiche mit Status und Aktionen.
- `07-rechte-live.png`: Rollenübersicht und Rollenformular.
- `08-module-live.png`: installierte Module.
- `09-schuljahr-zuordnungen-live.png`: aktives Halbjahr, Tutor- und
  Fachlehrkraftzuordnungen.
- `10-curriculum-importvorschau-live.png`: Curriculumfilter, Münzbudget,
  Suchfeld und sichere Importvorschau ohne Datei.

Nicht mutierende oder gefährliche Aktionen wurden nicht als erfolgreich
abgebildet. Das betrifft insbesondere Import bestätigen, Semesterwechsel,
Freigeben/Sperren, Löschen, Archivieren, Passwortwechsel, Rechteänderung und
echte Exporte.

Die sichtbaren Detail-/Bearbeiten-/QR-Dialogschaltflächen wurden nicht als
PASS für ihre Folgeansicht gewertet, wenn der Browserpfad nicht sauber ohne
Wartefehler abgeschlossen werden konnte. Es gibt dafür keinen irreführenden
Erfolgsscreenshot.
