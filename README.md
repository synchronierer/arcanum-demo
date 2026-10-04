# arcanum-demo

Public DEMO (separate test environment) for the Arcanum Learn Monitoring System.

## Public test access

This repository and the linked access list are public. Anyone may use the
published DEMO accounts to sign in to the DEMO service. The list contains
administration, teacher, and student accounts in that order; students are
sorted by class.

- [DEMO credentials PDF](./Arcanum_DEMO_Zugangsdaten.pdf)

The PDF contains only synthetic DEMO accounts (fictional test identities).
It contains no PROD credentials, private keys, tokens, or configuration
secrets. Four retained `demo.umbau.*` accounts are listed, but their
passwords are marked as unavailable because no authorized password source
exists; no password was guessed or reset.

## Reset notice

Resetting the shared DEMO removes changes made by all testers. Do not reset
the DEMO until an explicit confirmation is shown. After a reset, sign in
again with the published DEMO account for the required role and use the
accounts, classes, and synthetic grade-five test students listed in the PDF.

The public repository documents the access model, but it does not contain a
database dump or any PROD data. The current reset action is not published
until a current, integrity-checked DEMO baseline (verified database backup)
and a tested restore path are available.
