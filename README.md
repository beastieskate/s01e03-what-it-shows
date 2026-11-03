# MEGA.dev S01E03 — what it shows

This repository contains the support knowledge-base export, the signed `.svx` page for ticket #4471, and the rendered page the desk will see.

The export has 412 unique reports (427 rows including 15 duplicate rows). The two problems are:

- shared parser reads day-first dates as month-first: 379 reports
- booking-v3 date hint disagrees with tenant date order: 33 reports

Rendered page: [`rendered/kb/incidents/4471/index.html`](rendered/kb/incidents/4471/index.html)
