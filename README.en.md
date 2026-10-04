# Arcanum DEMO

Public DEMO (separate test environment) for the Arcanum learning system.

**Open the DEMO:** [https://arcanum-demo.dynv6.net](https://arcanum-demo.dynv6.net)

## Quick start

1. Open the DEMO address in a current browser. A laptop is recommended for the first tour, but it is not required. Tablets and smartphones are supported as well.
2. Open the [public credentials PDF](./Arcanum_DEMO_Zugangsdaten.pdf). It contains the usable administration, teacher, and student accounts.
3. Choose a role and sign in with the corresponding account.
4. Follow the [English DEMO handbook](./docs/guide.en.md). The complete German version is available in the [German handbook](./docs/handbuch.de.md).

The DEMO contains synthetic data (fictional test data only). Several people use the same environment, so changes to shared data may be visible to other visitors.

## DEMO screenshots

![Empty sign-in page of the public DEMO](docs/images/01-login.png)

*Empty sign-in page – credentials are entered only after choosing an account.*

![Student dashboard of a synthetic grade-five student](docs/images/02-schueler-dashboard-5a.png)

*Student dashboard with a subject, progress, and learning-path tiles.*

![Tutor view for class 5a](docs/images/04-tutor-5a.png)

*Tutor view (view for class mentors) showing the five synthetic students in 5a.*

## Public credentials

The credentials PDF is intentionally public and is meant only for this DEMO. It contains 138 usable accounts: 3 administration accounts, 12 teacher accounts, and 123 student accounts.

The DEMO has 142 accounts in total. Four technical `demo.umbau.*` accounts have no available authorized password source and are therefore not published as usable logins. PROD credentials (live-system credentials), private keys, tokens, and configuration secrets are not included.

## Resetting the DEMO

Resetting removes shared changes made by all testers. The verified baseline contains the published usable accounts, the classes, 20 synthetic students in 5a–5d, and their subject assignments.

The current reset path is an operator-controlled restore (performed manually by the responsible environment) and is not a web button. It was tested with a harmless temporary entry. A public web action with explicit confirmation is not yet part of the DEMO and is not claimed here.

## Components

- The Arcanum core provides sign-in, roles, student, teacher, and administration pages, curriculum (planned learning content), stages, and tasks.
- The Arcanum overlay is an additional display layer used by the student view.
- The Results plugin (result and progress extension) supports result and learning-progress views.
- The attendance plugin provides “Anwesenheit” and “Attendance verwalten”.
- Role and permission management controls roles and access rights.
- SOL planner, SOL student overviews, displays/signage, ScreenTinker, and WebUntis integrations are not part of this public DEMO or have not been verified as working here.

## Further documentation

- [Guided English handbook](./docs/guide.en.md)
- [Deutsches Handbuch](./docs/handbuch.de.md)

---

**Deutsche Version:** [README.md](./README.md)
