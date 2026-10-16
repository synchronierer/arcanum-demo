# Internes Funktionsinventar – DEMO-Rundgänge

Stand: 16.10.2026, Live-URL `https://arcanum-demo.dynv6.net/login`, Browser
1440 px. Passwörter, Sitzungen und geheime Serverinformationen sind nicht
Bestandteil dieses Nachweises.

## Baseline

Die veröffentlichte Zugangsdaten-PDF wurde direkt von GitHub (`origin/main`)
bezogen und verwendet. Empfohlene Konten: `anton.apfel` (Schüler),
`dora.dinkel` (Lehrkraft/Tutor 6d), `ada.ananas` (Administration). Die
Live-Demo meldete 209 Schüler, 81 Lehrkräfte, 8 Klassen, 21 Fächer und das
aktive Halbjahr `2026_27_HJ1`. Attendance zeigte 222 Schüler, was die
abweichende Anwesenheitsbasis ausdrücklich dokumentiert.

## Rollen-/Kontenmatrix

| Rolle | Testkonto | Demonstrierte Funktionen | Anmeldung | Besonderheiten |
|---|---|---|---|---|
| Schüler | `anton.apfel` / Anton Apfel, 6a | Dashboard, Fachkarten, Aktionen, Avatar, Etappenstatus, Ergebnisroute | PASS | 0 Münzen; Hilfe aktiv; alle vier Etappenzähler 0 |
| Lehrkraft/Tutor | `dora.dinkel` / Dora Dinkel | Cockpit, 2 Unterrichtskontexte, Curriculum, Fortschritt, GN, Tutor 6d, Attendance | PASS | Tutorbereich zeigte 25 Schüler |
| Administration | `ada.ananas` / Ada Ananas | Dashboard, Schuldaten, Zuordnungen, Curriculum, Attendance, Rechte, Module | PASS | öffentlicher Demo-Admin; keine Mutationen |

## Routen- und Funktionsmatrix

Status bedeutet: PASS = lesend sichtbar und geprüft; FAILED = erreichbar,
aber fachlich fehlgeschlagen; NICHT_SICHER_AUSFÜHRBAR = absichtlich nicht
mutiert.

| Rolle | Seite/Unterbereich | Bedienelemente/Zustand | Status | Screenshot/Doku |
|---|---|---|---|---|
| Schüler | `/dashboard` Profil | Klasse, Graduierung, Rang, Münzen, Avatar, Abmelden | PASS | `01-dashboard-live.png` |
| Schüler | `/login` | Benutzername/Passwortfelder, Anmeldung ohne ausgefülltes Passwort | PASS | `00-anmeldung-live.png` |
| Schüler | Fachkarten | Notengrenzen, Zwischenstand, Prognosehinweis, reguläre Fächer, WPF | PASS | Schüler §3 |
| Schüler | Aktionen | Hilfe, Partner, Experiment, GN; aktiv/inaktiv | PASS | Dashboard |
| Schüler | Etappen | Offen, Aktuell, Bestanden, Gesperrt; Livezähler 0/0/0/0 | PASS | Schüler §6 |
| Schüler | Avatar | Auswahlfenster ohne Speichern | PASS | `02-avatar-dialog-live.png` |
| Schüler | `/results` Schatzkammer | Loader bleibt stehen, Ladefehler nach 1/5 s | FAILED | bewusst kein Erfolgsbild |
| Schüler | Logout | Abmelden | PASS | Textinventar |
| Lehrkraft | `/dashboard#overview` | Halbjahr, Lerngruppen, Fächer, Kontexte | PASS | `01-cockpit-live.png` |
| Lehrkraft | `#curriculum` | Kontextwahl, Budgets, zentrale/flexible Themen, Status, variable Münzen | PASS | `02-themen-etappen-live.png` |
| Lehrkraft | `#student-progress` | gefüllte Schülerliste, sichtbarer Details-Button, Lernstand und Signale | PASS/NI-SA | `03-schuelerfortschritt-live.png`; Detaildialog nicht als PASS gewertet |
| Lehrkraft | `#schoolwide-stage-overview` | GN-Bereitschaften, Fehlversuche, fünf Lesefilter | PASS | `04-gelingensnachweise-live.png` |
| Lehrkraft | `#tutor-area` | Klasse 6d, 25 Schüler, Fächer, Münzen, Noten, Verlauf, PDF | PASS | `05-tutorbereich-live.png` |
| Lehrkraft | `/attendance` | Datum, Zeitbezug, Standort, Status, Klasse, Suche, 222 Schüler | PASS | `06-anwesenheit-live.png` |
| Lehrkraft | Mutationen | Freigeben, Sperren, Bestätigen, Speichern, Graduierung ändern | NICHT_SICHER_AUSFÜHRBAR | Lehrkraft §9 |
| Admin | `/dashboard` | 209/81/8/21, Navigation, aktives HJ | PASS | `01-dashboard-live.png` |
| Admin | `/manage_students` | edu.sys/CSV, Liste, Fach/Status/Klasse/Suche, Exporte, Kontenaktionen | PASS | `02-schuelerverwaltung-live.png` |
| Admin | `/manage_teachers` | Formular, CSV, Suche, Export, Bearbeiten, Passwort | PASS | `03-lehrkraefte-live.png` |
| Admin | `/manage_classes` | Name/Jahrgang, 8 Klassen, Bearbeiten/Archivieren | PASS | `04-klassen-live.png` |
| Admin | `/manage_subjects` | 21 aktive Fächer, Typ, Kl.5/6, Aktionsmenü | PASS | `05-faecher-live.png` |
| Admin | Schuljahr/Zuordnungen | HJ aktiv, Tutor 1/2, Jahrgang, Lehrkraft-/WPF-Auswahl | PASS | Admin §4 |
| Admin | Curriculum/Import | Themen/Etappen, neue Themen, Vorschau, Import bestätigen | PASS/NI-SA | Admin §5 |
| Admin | `/attendance-admin` | 7 QR-Bereiche, Typ/Code/Status/Reihenfolge, QR anzeigen | PASS | `06-attendance-admin-live.png` |
| Admin | `/attendance` | schulweite Filter und Liste | PASS | Inventar |
| Admin | `/manage_permissions` | teacher/student/admin, Rollenformular | PASS | `07-rechte-live.png` |
| Admin | `/plugins` | 5 installierte Module | PASS | `08-module-live.png` |
| Admin | Dialoge/Formulare | sichtbare Bearbeiten-/QR-/Rollen-/Importelemente; keine Speicherung | NI-SA | keine Mutation ausgeführt |
| Admin | kritische Aktionen | Semesterwechsel, Import, Löschen, Rechte, Passwort, Export | NI-SA | nicht mutiert |

## Responsive

1440 px: alle gespeicherten Aufnahmen lesbar und ohne horizontalen Überlauf.
768 px ist laut Projekt-Browsergate unterstützt. 390 px bleibt als bekannte
Einschränkung mit möglichem seitlichem Scrollen dokumentiert; es wurde deshalb
kein 390-px-Bild als Qualitätsbeleg veröffentlicht.
