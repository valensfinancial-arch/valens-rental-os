# Rental Property Management OS
### Valens Capital · Interactive portfolio workspace

**Live site:** https://valensfinancial-arch.github.io/valens-rental-os/

An original, self-contained rental property CRM inspired by the public information architecture of Ziko Templates’ *Rental Property Management OS* (Gumroad listing). This is not a copy of the paid Notion file. It is a richer, fully interactive workspace with the same module map and a closely related visual language.

## Open
Open `index.html` in a modern browser. No install, no account, no server required.

Live URL after Pages builds:
https://valensfinancial-arch.github.io/valens-rental-os/

Optional local server:
```
python3 -m http.server 8765 --directory .
```

## Modules
1. Dashboard — occupancy, rent collected, NOI, late balances, work orders, applicant pipeline widget
2. Properties — gallery cards with rent, NOI, and cap rate
3. Tenants — directory with credit, income, and payment history
4. Applicants — first-qualified leasing pipeline
5. Leases — term table with 90/60/30 countdown chips
6. Rent Payments — rent roll with one-click Mark Paid
7. Expenses — category ledger that feeds the dashboard rings
8. Maintenance Requests — New / Scheduled / In Progress / Done board
9. Vendors — trade directory with insurance dates
10. Inspections — score and result log
11. Documents — expiry radar (Current / Expiring / Expired)

## Applicant pipeline
Stages: Inquiry → Applied → Screening → Approved → Signed, plus Denied / Withdrawn.

Published criteria (shown on the board):
- First complete file wins (not first inquiry)
- Income ≥ 3× asking rent
- Credit floor 650 when a report is on file
- Screening checklist: photo ID, income docs, credit consent + report, prior landlord, background, pet/occupancy docs

Open an applicant drawer to toggle checklist items, move stages, or **Convert to tenant + lease**. Conversion creates a tenant record, a 12-month draft lease (deposit = 1 month rent), and marks the unit occupied when it is vacant.

Fair Housing / FCRA: the file does not collect protected-class fields. Denials should cite the written policy only. If a consumer report was used, send an adverse-action notice.

## Improvements versus a static Notion OS
- Working navigation and record drawers
- Mark Paid updates collection totals immediately
- Quick Actions that open a real add-record form
- Cap rate and cash-on-cash on every property
- Maintenance kanban with status changes
- Document expiry states
- Search and status filters on every module
- Sample Miami-area portfolio persisted to `localStorage`
- Header export / import backup

## Sample portfolio
Cedar Ridge Court, Capitol Hill Townhome, Maple Grove Residence, Liberty Landing 9C, Palmetto Place 305, Oak & Pine Duplex, Magnolia Court, Riverfront Lofts, Sunset Villas, Desert Bloom Suite 12.

Reset demo data by clearing site data for the page (localStorage key `valens-rental-os-v3`).

## Keep updating from Grok
This repo is the live source. Ask Grok to change the CRM and it will push to `main`. GitHub Pages republishes automatically.
