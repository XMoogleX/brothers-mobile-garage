# Brothers Mobile Garage — Shop Management Prototype

A no-dependency browser prototype for customer, vehicle, and estimate tracking.

## Limitations
- **Demo only:** Data is saved to localStorage on one browser/device. No sync, authentication, backups, access controls, or secure server-side storage. **Do not use real customer information.**
- Tax is a manual estimate entry, not a jurisdiction-specific calculation.
- Invoices are a read-only view of approved estimates; payment processing, official invoice numbers, PDF export, and edits are not implemented.
- No parts compatibility verification, warranties, or accounting integration.

## Production roadmap
1. Database and authenticated users with role-based access.
2. Server-side validation, secure data handling, backups, and audit history.
3. Editable estimate line items, approvals, unique invoice numbers, payment tracking, and PDF output.
4. Jurisdiction-appropriate tax handling and customer-supplied-parts terms.

## Pricing logic (v1.1)
- Hourly or flat-rate labor per estimate.
- Parts selling price = parts cost × (1 + markup percentage / 100).
- Configure applicable sales tax rate and taxable categories; defaults to 0% and none selected until verified.
- Quote total is rounded **up** to the next whole dollar. The adjustment (0–99 cents) is explicitly shown internally.
- The quote preview displays a tax-inclusive final customer total.
- Estimates are still demo-only in browser localStorage; no authentication or backup.
