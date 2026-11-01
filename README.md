# Security Deposit and FDR Portal

**Smart India Hackathon 2026 | Problem Statement SIH26265 | Software | Team 555_UDBHAV**

A web portal that lets departments, contractors and officers manage security deposits held as Fixed Deposit Receipts (FDRs) in one place, from submission to release.

**Live demo:** https://YOUR-USERNAME.github.io/sih26265-fdr-portal/

![Dashboard](screenshots/dashboard.png)

## The problem

Security deposits are often kept as paper FDRs. Receipts are checked by eye, liens are not tracked, and maturity dates are missed. Refunds are slow and officers have no single view of what is held.

## What the portal does

- **Digital submission:** contractors add FDR details and the receipt.
- **Bank verification:** each FDR is confirmed with the issuing bank.
- **Lien register:** the department's lien is recorded and tracked.
- **Maturity alerts:** reminders at 30, 15 and 7 days before maturity.
- **Release workflow:** release is approved after the defect liability period ends.
- **Audit trail:** every action is timestamped.
- **Dashboard:** totals, status filters, search, upcoming maturities, deposits per bank and live alerts.
- **Roles:** switch between accounts officer, contractor and bank to see what each can do.

## Current status

| Part | Status |
|---|---|
| Frontend dashboard | Working demo: add FDRs, bank verification, lien, renewal, release, audit trail, reports (saved in browser) |
| Backend (FastAPI) | Folder structure ready, files are empty |
| Bank API, OCR | Planned |

All names, amounts and counts shown in the dashboard are sample data.

## Tech stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript (prototype). Planned: React 18, TypeScript, Vite, Tailwind CSS |
| Backend | Python FastAPI, Uvicorn, Pydantic |
| Database | PostgreSQL / Supabase |
| AI | OCR for receipts, rule-based checks |
| DevOps | Docker, Docker Compose |

## Project structure

```
sih26265-fdr-portal/
├── frontend/        Working demo app (index.html)
├── backend/         FastAPI app (files created, empty)
│   └── app/         api, models, services, core
├── docs/            Copy of the dashboard served by GitHub Pages
├── presentation/    SIH presentation (.pptx)
├── screenshots/     Images used in this README
└── docker-compose.yml
```

## Run locally

Open `frontend/index.html` in any browser. No install needed.

## Publish on GitHub Pages

1. Open the repository **Settings**, then **Pages**.
2. Under **Branch**, choose `main` and the `/docs` folder, then save.
3. After a minute the live link appears on the same page.

## Team

Team 555_UDBHAV, Smart India Hackathon 2026.

## License

MIT
