# Brothers Mobile Garage — Shop Management Prototype

A no-dependency browser prototype for customer, vehicle, and estimate tracking.

## Run
Open `index.html` in a browser, or run `python -m http.server 8000` in this directory and visit http://localhost:8000.

## Limitations
- **Demo only:** Data is saved to localStorage on one browser/device. No sync, authentication, backups, access controls, or secure server-side storage. **Do not use real customer information.**
- Tax is a manual estimate entry, not a jurisdiction-specific calculation.
- Invoices are a read-only view of approved estimates; payment processing, official invoice numbers, PDF export, and edits are not implemented.
- No parts compatibility verification, warranties, or accounting integration.

## Recommended production roadmap
1. Database and authenticated users with role-based access.
2. Server-side validation, secure data handling, backups, and audit history.
3. Editable estimate line items, approvals, unique invoice numbers, payment tracking, and PDF output.
4. Jurisdiction-appropriate tax handling and customer-supplied-parts terms.

## Suggested repository name
`brothers-mobile-garage`
