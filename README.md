# Gudditheking Loan Management PRO — GitHub Pages

A responsive, browser-based loan management application built with **HTML, CSS and vanilla JavaScript**. It is adapted to the uploaded Excel workbook `MAREJESHO YA MKOPO KWA SIKU 30`.

## Live deployment with GitHub Pages

1. Create a new GitHub repository, for example `gudditheking-loan-management`.
2. Upload `index.html`, the `assets/` folder and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for GitHub Pages to publish the site. Your site address will be shown in Settings → Pages.

You can also use GitHub's **Add file → Upload files** to upload the package contents.

## Features

- Dashboard with borrower, principal, total due, collection and outstanding totals.
- Borrower directory with contact details.
- Loan issuance with principal, entered interest value and agreed total amount due.
- Repayment recording, collection date, receipt/reference and schedule day 1–31.
- Automatic loan collection and balance calculations.
- Borrower-level statements with print / Save as PDF.
- Portfolio reports.
- CSV exports for borrowers, loans and repayments (Excel compatible).
- JSON backup and restore.
- Responsive layout for mobile, tablet and desktop.

## Data and security limitations

This is a **static GitHub Pages edition**. Records are saved in the browser's `localStorage` on the device and browser being used.

- It does not provide a shared central database. Different employees/devices do not see each other's records.
- Clearing browser storage, changing browser or device, or using private browsing may make records unavailable. Download backups regularly.
- There is no secure user login or role-based access in this static version. Do not treat GitHub Pages/localStorage as secure storage for sensitive financial or personal information.
- For multi-user production use, use the PHP/MySQL PRO version or connect this frontend to a properly secured backend with authentication, authorization, HTTPS, audit logs and backups.

## Workbook mapping

The app follows the workbook's fields:
- `S/N`
- `FULL NAME`
- `NAMBA YA SIMU`
- `KIASI CHA MKOPO`
- `RIBA`
- `JUMLA YA MKOPO`
- daily repayment columns `1` to `31`
- `JUMLA YA MAREJESHO`

The workbook does not define a universal interest formula or a complete due-date policy. Therefore, the app stores the interest value and asks the operator to enter the agreed total amount due rather than inventing a formula.

## Project structure

```text
Gudditheking_GitHub/
├── index.html
├── README.md
└── assets/
    ├── app.js
    └── style.css
```

## Local preview

Open `index.html` in a modern browser. No build step or package installation is required.
