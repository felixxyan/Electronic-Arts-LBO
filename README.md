# Electronic Arts — LBO Model

A leveraged buyout model for a hypothetical take-private of Electronic Arts (NASDAQ: EA) by a sponsor consortium (Silver Lake, PIF, and Affinity Partners). Combines a full sources & uses build, purchase price allocation, and a three-statement operating model with sponsor returns analysis and sensitivity tables. Also includes a standalone WACC and DCF valuation to cross-check the entry price.

 - Currency: USD, millions (except per-share figures)
 - Transaction / pricing date: September 25, 2025
 - Historical years: FY2021–FY2025 · Projection years: FY2026–FY2030 · Assumed exit: March 31, 2030

## Tab guide

| Tab | Purpose |
|---|---|
| **LBO** | Deal control page. General inputs, sources & uses of funds, entry valuation (offer price / EBITDA multiple), financing fees, exit valuation, sponsor/co-investor returns (cash-on-cash, IRR), returns summary, and sensitivity tables (offer price vs. hurdle rate, IRR vs. leverage/entry multiple, IRR vs. leverage/offer price). |
| **Financials** | EA standalone three-statement model (income statement and supporting schedules), with a circularity breaker switch for interest-driven circular references. |
| **Pro Forma** | Purchase price allocation and pro forma adjustments — asset write-ups to PP&E and intangibles, resulting incremental D&A and deferred tax liabilities, and pro forma balance sheet adjustments. |
| **WACC** | Cost-of-capital build: risk-free rate, market risk premium, levered beta, and the resulting WACC, used as a reference discount rate. |
| **DCF** | Standalone discounted cash flow valuation (unlevered free cash flow build off the Financials tab), used to sanity-check the LBO entry price independent of the financing structure. |

## Methodology

Sources & uses → Purchase price allocation → Pro forma financials → Debt paydown → Exit → Returns. The model is fully linked and formula-driven: change an assumption on the LBO tab and it flows through the pro forma statements, debt schedules, and sponsor returns output.

- **Entry structure:** Offer price of $210.00/share (~24.8% premium), implying ~20.9x LTM EBITDA and an enterprise value of ~$53.8B. Financed with a 7.0x EBITDA term loan, PIF equity rollover, sponsor equity, and excess cash on the balance sheet.
- **Purchase price allocation:** Target PP&E and intangible assets are written up to fair value, generating incremental depreciation/amortization and deferred tax liabilities that flow into the pro forma income statement.
- **Debt paydown & exit:** Debt is amortized/paid down through the projection period; exit is modeled at March 31, 2030 across a range of exit EBITDA multiples (21.5x–41.5x, base case 31.5x).
- **Returns:** Cash-on-cash and IRR are computed for each capital tranche (term loan, PIF rollover, sponsor equity) at exit, with a returns summary at the base-case exit multiple and two-way sensitivity tables flexing offer price vs. sponsor hurdle rate and sponsor IRR vs. leverage/entry multiple or leverage/offer price.
- **DCF cross-check:** A separate WACC-discounted DCF (unlevered free cash flow, standalone WACC) provides an independent valuation reference alongside the LBO entry multiple.

## Conventions

- Blue text — hardcoded inputs / assumptions
- Black text — formulas
- Green text — links from another sheet
- "Circ Breaker" toggle on the Financials tab — switches off circular references (enable iterative calculation in Excel if formulas show circular reference warnings)
- On the LBO tab, sensitivity tables under "EXPLICIT EBITDA" vs. "EXPLICIT OFFER PRICE" approaches require the corresponding valuation approach to be selected for the data table to populate

## How to use

1. Open in Excel (or LibreOffice Calc / Google Sheets).
2. Start on the LBO tab for the headline deal terms, sponsor returns, and sensitivity tables.
3. Adjust offer price, leverage (term loan/EBITDA turns), or exit multiple assumptions on the LBO tab — everything downstream recalculates automatically.
4. Check the WACC and DCF tabs to compare the LBO entry multiple against an independent cash-flow-based valuation.

## Disclaimer

This model is a hypothetical modeling exercise for educational and illustrative purposes only. It does not represent an actual, announced, rumored, or endorsed transaction, and none of the assumptions, projections, or outputs should be relied upon for investment or business decisions.
