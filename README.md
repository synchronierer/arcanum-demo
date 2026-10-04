# arcanum-demo

Public DEMO (separate test environment) for the Arcanum Learn Monitoring System.

DEMO website: https://arcanum-demo.dynv6.net

## Public test access

This repository and the linked access list are public. Anyone may use the
published DEMO accounts to sign in to the DEMO service. The list contains
administration, teacher, and student accounts in that order; students are
sorted by class.

- [DEMO credentials PDF](./Arcanum_DEMO_Zugangsdaten.pdf)

The PDF contains 138 usable synthetic DEMO accounts (fictional test
identities): 3 administration accounts, 12 teacher accounts, and 123 student
accounts. The four retained `demo.umbau.*` accounts are intentionally omitted
because their passwords are unavailable; no password was guessed or reset.
The PDF contains no PROD credentials, private keys, tokens, or configuration
secrets.

## Öffentliche Nutzung / Public use

Dieses Repository und die PDF sind absichtlich öffentlich. Alle Besuchenden
dürfen die aufgeführten DEMO-Konten zum Ausprobieren verwenden. Die
Zugangsdaten gehören ausschließlich zur getrennten DEMO und nicht zu PROD.

This repository and the PDF are intentionally public. All visitors may use
the listed DEMO accounts for testing. The credentials belong only to the
separate DEMO and are not PROD credentials.

## DEMO zurücksetzen / Reset the DEMO

Das Zurücksetzen der gemeinsam genutzten DEMO entfernt Änderungen aller
Testenden. Der aktuell geprüfte Wiederherstellungsstand enthält die 138
verwendbaren öffentlichen Konten, die Klassen, die 20 synthetischen Schüler
in 5a–5d und deren Fachzuordnungen. Nach dem Zurücksetzen meldet man sich mit
einem Konto aus der PDF erneut an.

Resetting the shared DEMO removes changes made by all testers. An explicit
confirmation is required before the reset. Afterward, sign in again with a
published DEMO account for the required role.

The current reset mechanism is an operator-controlled restore of the
integrity-checked DEMO baseline (verified database backup). It was tested with
a harmless temporary entry, which disappeared after restore; the baseline
remained at 124 students, 14 teachers, and 4 administrators with 756 known
foreign-key violations (database references to missing rows), unchanged.
It is not yet exposed as a web action for public DEMO administrators, so no
claim is made here that visitors can trigger it from the website. A database
dump and PROD data are not stored in this repository.

The current reset mechanism is not a public self-service action because the
required confirmation and authorization screen still need to be implemented.
