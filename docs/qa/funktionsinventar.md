# Internes Funktionsinventar – DEMO-Rundgänge

Stand: 16.10.2026, unabhängige Zweitabnahme, Live-URL
`https://arcanum-demo.dynv6.net/login`, Browserbreite 1440 px. Passwörter,
Sitzungen und geheime Serverinformationen gehören nicht in diesen Nachweis.

## Baseline und Konten

Die aktuelle GitHub-Zugangsdaten-PDF war die einzige Kontoquelle. Die
Demo-Baseline zeigte 209 Schüler, 81 Lehrkräfte, 8 Klassen, 21 Fächer und das
aktive Halbjahr `2026_27_HJ1`. Anwesenheit zeigte 222 Datensätze; diese
abweichende Anzeige wird nicht mit der Schülerverwaltung gleichgesetzt.

| Rolle | Konto | Gezeigte Zustände | Anmeldung |
|---|---|---|---|
| Schüler | `anton.apfel` | leerer Lernstand, Dashboard, Avatar, Statuskacheln, Fehlerfall `/results` | PASS |
| Schüler | `berta.banane` | 7 Münzen, Rang 1/97, Mathematik/WPF je 1 bestandene Etappe, variables Logbuch | PASS |
| Schüler | `dora.kakao` | unabhängige Wiederholung des `/results`-Fehlers | PASS; Funktion FAILED |
| Lehrkraft/Tutor | `dora.dinkel` | Cockpit, 2 Kontexte, Curriculum, gefüllter Fortschritt/GN, Tutor 6d | PASS |
| Administration | `ada.ananas` | Dashboard, Schuldaten, Schuljahr, Curriculum, Attendance, Rechte, Module | PASS |

## Einzelne Prüffunktionen

`PASS` bedeutet ausschließlich: genau dieses lesende Verhalten wurde im
Browser beobachtet. Ein sichtbarer Button ohne Ausführung ist kein PASS.

| Nr. | Rolle/Konto | Seite / Unteransicht | Bedienelement oder Zustand | Tatsächlich beobachtet | Screenshot | Doku | Status |
|---:|---|---|---|---|---|---|---|
| S01 | Schüler / Anton | `/login` | Loginfelder und Anmeldung | Dashboard geladen | `schueler/00-anmeldung-live.png` | Schüler §1 | PASS |
| S02 | Schüler / Anton | `/dashboard` | Profil, Klasse, Graduierung | 6a, Neustarter, Kennung sichtbar | `schueler/01-dashboard-live.png` | Schüler §2 | PASS |
| S03 | Schüler / Anton | Fachkarten | Notengrenzen/Zwischenstand | Grenzen und Note 6 sichtbar | `schueler/01-dashboard-live.png` | Schüler §2–3 | PASS |
| S04 | Schüler / Anton | Fachkarte | Avatar bearbeiten | Dialog geöffnet, nicht gespeichert | `schueler/02-avatar-dialog-live.png` | Schüler §4 | PASS |
| S05 | Schüler / Anton | Fachkarte | Hilfe/Partner/Experiment/GN | Aktiv/inaktiv sichtbar, Klick nicht ausgeführt | `schueler/01-dashboard-live.png` | Schüler §5 | PASS |
| S06 | Schüler / Anton | Fachkarte | Offen/Aktuell/Bestanden/Gesperrt | 0/1/1/0 nach regulärem Neubau | `schueler/01-dashboard-live.png` | Schüler §6 | PASS |
| S07 | Schüler / Berta | `/dashboard` | Gesamtmünzen/Rang | 1 Münze, Klasse 6d | `schueler/03-berta-dashboard-live.png` | Schüler §3 | PASS |
| S08 | Schüler / Berta | Mathematik-Karte | verdiente Münzen | 1 Münze, 1 bestanden, 1 Fehlversuch | `schueler/04-berta-mathematik-live.png` | Schüler §6 | PASS |
| S09 | Schüler / Berta | Mathematik-Karte | Zwischenstand/Notengrenze | Note 6, 19 bis Note 5 | `schueler/04-berta-mathematik-live.png` | Schüler §6 | PASS |
| S10 | Schüler / Berta | WPF-Karte | individuelles Fach | 4 Münzen, 1 bestanden | `schueler/05-berta-wpf-live.png` | Schüler §7 | PASS |
| S11 | Schüler / Berta | `/results` Mathematik | Erfolgslogbuch | 1 Münze, zentrale Etappe sichtbar | `schueler/06-berta-schatzkammer-live.png` | Schüler §8 | PASS |
| S12 | Schüler / Dora Kakao | `/results` Deutsch | Etappe, Thema, Wert | zentrale Deutsch-Etappe, +3 sichtbar | — | Schüler §8 | PASS |
| S13 | Schüler / Anton | `/results` | Fortschritzdaten laden | HTTP 200, 1 Mathe-Münze sichtbar | — | Schüler §8 | PASS |
| S14 | Schüler / Dora Kakao | `/results` | Fortschritzdaten laden | HTTP 200, Deutsch-Erfolg sichtbar | — | Schüler §8 | PASS |
| S15 | Schüler / öffentliche Konten | Fachkarten | Zeugnisprognose | bei wenigen Etappen noch nicht berechenbar | — | Schüler §6/8 | OPEN |
| L01 | Lehrkraft / Dora | Cockpit | Halbjahr/Kontexte | 2026_27_HJ1, 6d GL/Mathematik | `lehrkraft/01-cockpit-live.png` | Lehrkraft §1–2 | PASS |
| L02 | Lehrkraft / Dora | Curriculum | zentrale/flexible Themen | 63+20, Rahmen 100, Grenze 105 | `lehrkraft/02-themen-etappen-live.png` | Lehrkraft §3 | PASS |
| L03 | Lehrkraft / Dora | Schülerfortschritt | Kontext laden | mehrere Schüler und Signale | `lehrkraft/03-schuelerfortschritt-live.png` | Lehrkraft §4 | PASS |
| L04 | Lehrkraft / Dora | Schülerfortschritt | Details erster Schüler | Anton Banane, Etappen/Bewertungen sichtbar | `lehrkraft/07-schueler-detail-live.png` | Lehrkraft §4 | PASS |
| L05 | Lehrkraft / Dora | Schülerdetail | Leistungsbestätigung | Anton, Berta und Dora regulär bestätigt; Berta mit Fehlversuch | — | Lehrkraft §4/9 | PASS |
| L06 | Lehrkraft / Dora | GN | fünf Lesefilter | Bereitschaften und 1x Fehlversuch sichtbar | `lehrkraft/04-gelingensnachweise-live.png` | Lehrkraft §5 | PASS |
| L07 | Lehrkraft / Dora | Tutor 6d | Übersicht laden | 25 Schüler, Fachmünzen/Noten | `lehrkraft/05-tutorbereich-live.png` | Lehrkraft §6 | PASS |
| L08 | Lehrkraft / Dora | Tutor 6d | Verlauf anzeigen | Zeile markiert, keine separate Ansicht/kein Fehler | `lehrkraft/08-tutorverlauf-live.png` | Lehrkraft §6 | FAILED |
| L09 | Lehrkraft / Dora | Attendance | Filter und Suche | Felder und 222 Datensätze sichtbar | `lehrkraft/06-anwesenheit-live.png` | Lehrkraft §7 | PASS |
| L10 | Lehrkraft / Dora | Curriculum/Attendance | Speichern/Bestätigen | absichtlich nicht ausgeführt | — | Lehrkraft §9 | NICHT_SICHER_AUSFÜHRBAR |
| A01 | Admin / Ada | Dashboard | Kennzahlen/Navi | 209/81/8/21, aktive HJ | `administration/01-dashboard-live.png` | Admin §1 | PASS |
| A02 | Admin / Ada | Schülerverwaltung | Fach/Status/Klasse/Suche | Filter und 209er Liste sichtbar | `administration/02-schuelerverwaltung-live.png` | Admin §2 | PASS |
| A03 | Admin / Ada | Lehrkräfteverwaltung | Suche/Formular/CSV | 81er Liste und Vorschaufelder | `administration/03-lehrkraefte-live.png` | Admin §2 | PASS |
| A04 | Admin / Ada | Klassenverwaltung | Klassenliste | 5a–5d, 6a–6d sichtbar | `administration/04-klassen-live.png` | Admin §2 | PASS |
| A05 | Admin / Ada | Fächerverwaltung | Typ/Aktivität/Aktionsmenü | 21 Fächer und Menüs | `administration/05-faecher-live.png` | Admin §3 | PASS |
| A06 | Admin / Ada | Schuljahr | Halbjahr/Jahrgang | aktives HJ, Tutor-/Fachmatrizen | `administration/09-schuljahr-zuordnungen-live.png` | Admin §4 | PASS |
| A07 | Admin / Ada | Schuljahr | individuelle Fächer/WPF | Ansicht/Filter sichtbar, keine Änderung | `administration/09-schuljahr-zuordnungen-live.png` | Admin §4 | PASS |
| A08 | Admin / Ada | Curriculum | Fach/HJ/Jahrgang/Suche | Filter und Ergebnistabelle sichtbar | `administration/10-curriculum-importvorschau-live.png` | Admin §5 | PASS |
| A09 | Admin / Ada | Curriculum-Import | Vorschau ohne Datei | erreichbar, keine Datei | `administration/10-curriculum-importvorschau-live.png` | Admin §5 | PASS |
| A10 | Admin / Ada | Curriculum-Import | Import bestätigen | nicht ausgeführt | — | Admin §5 | NICHT_SICHER_AUSFÜHRBAR |
| A11 | Admin / Ada | Attendance-admin | QR-Bereiche | 7 Bereiche, Status/Typ/Reihenfolge | `administration/06-attendance-admin-live.png` | Admin §6 | PASS |
| A12 | Admin / Ada | Rechte | Rollenliste/Formular | teacher/student/admin sichtbar | `administration/07-rechte-live.png` | Admin §7 | PASS |
| A13 | Admin / Ada | Rechte | Rollendetails | keine separate Detailansicht nachgewiesen | — | Admin §7 | NICHT_SICHER_AUSFÜHRBAR |
| A14 | Admin / Ada | Module | Module expandieren | nur zusammengeklappte Liste belastbar | `administration/08-module-live.png` | Admin §7 | NICHT_SICHER_AUSFÜHRBAR |
| A15 | Admin / Ada | kritisch | Löschen/Rechte/Passwort/HJ | nicht mutiert | — | Admin §8 | NICHT_SICHER_AUSFÜHRBAR |

## Responsive- und Sicherheitsbefund

1440 px: neue Aufnahmen wurden gespeichert und visuell erneut geöffnet. 768 px
ist als unterstützte Breite dokumentiert; 390 px kann seitlich scrollen, daher
wurde kein mobiles Bild als Erfolgsbeleg veröffentlicht. Die Bilder enthalten
nur synthetische DEMO-Identitäten und keine Passwörter, Tokens oder Freitexte.
