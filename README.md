# MEGA.dev S01E03 — what it shows

This repository contains the support knowledge-base export, the signed `.svx` page for ticket #4471, and the rendered page the desk will see.

The export has 412 unique reports (427 rows including 15 duplicate rows). The two problems are:

- shared parser reads day-first dates as month-first: 379 reports
- booking-v3 date hint disagrees with tenant date order: 33 reports

Signed review source: [`support-kb/src/routes/kb/incidents/4471-review/+page.svx`](support-kb/src/routes/kb/incidents/4471-review/+page.svx)

Rendered review: [`rendered/kb/incidents/4471-review/index.html`](rendered/kb/incidents/4471-review/index.html)

The exported incident page is preserved as historical evidence; our signed review is a separate new KB page.

## Engineering outcome

The course's live desk update marks #4471 closed on 5 October 2026:

- [Parser issue #1](https://github.com/beastieskate/s01e03-what-it-shows/issues/1): fixed by `fix(dates): parse dd/mm for eu locales`; closed as completed.
- [Hint issue #2](https://github.com/beastieskate/s01e03-what-it-shows/issues/2): won't fix because the booking-v3 form was retired; closed as not planned.

These are separate outcomes. A closed parent ticket does not mean that every merged problem was fixed.
