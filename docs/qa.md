# Prototype verification

Verified in headless Chromium using Playwright, with desktop 1440×1000 and mobile 390×844 viewports.

## Passed
- All 14 routes (overview plus 13 modules) render without browser JavaScript errors.
- Product search matches alternate codes; product details show all three codes and packaging hierarchy.
- Product creation starts with zero stock.
- Two ceramic-mug cartons convert to 96 individual units on a purchase order.
- Dispatching a 48-unit order reduces both on-hand and reserved stock by 48.
- Partial GRV acceptance of 120 lamps updates stock from 38 to 158 and purchase status to partially received.
- A partial customer payment updates invoice paid amount and status.
- Supplier bill creation and full payment work locally.
- A newly posted journal appears as matching debit and credit rows in the general ledger.
- Client creation persists through reload.
- Accounting tabs and trial-balance report open correctly.
- Mobile navigation opens/closes, forms fit the viewport, no page-level horizontal overflow.
- Full currency metrics remain visible after reducing the mobile metric type size.
- Desktop dashboard, product detail, mobile dashboard and mobile form screenshots visually reviewed against the design lock.

## Boundaries
No real integrations, tax validation, authentication, server persistence or production accounting is implemented. Financial reports and dashboard trends are illustrative snapshots. Mobile tables intentionally scroll horizontally. Long forms scroll inside the dialog with a sticky header. Browser print/save-PDF is available but printer-specific pagination was not validated.

The original sample data was restored after verification. Verification tooling is kept outside the repository; the shipped platform has no dependencies.
