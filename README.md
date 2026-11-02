# Three-Statement Model and DCF: Berger Paints India

An Excel model for Indian listed companies: income statement, balance sheet and cash flow statement, supporting schedules, ratios, integrity checks and a DCF valuation. Berger Paints India (NSE: BERGEPAINT) is the worked example.

All amounts are in INR Crore unless stated.

## What is in this repo

| File | What it is |
|---|---|
| `Three_Statement_Model_India_v3.xlsm` | The macro-enabled Excel model |
| `Berger_Paints_DCF_LinkedIn.pdf` | 10-slide summary of the Berger Paints valuation |

## What the model does

- Pulls 12 years of annual consolidated historicals from Screener.in when you click the fetch button
- Forecasts five years with growth that fades towards a long-term rate, with Base, Bull and Bear scenarios
- Builds linked income statement, balance sheet and cash flow statement, with working capital, fixed asset, debt, other income and equity schedules
- Runs ratios and model integrity checks (the Cover sheet shows OK when the statements tie)
- Values the company with an FCFF DCF: CAPM cost of equity, WACC, mid-year discounting, a terminal value, an equity bridge and a WACC vs terminal growth sensitivity table
- Uses no circular references

## Sheets

Cover, Assumptions, IS, BS, CF, Schedules, Ratios, Data, DCF, Raw_Data.

## How to use

1. Download `Three_Statement_Model_India_v3.xlsm`.
2. Right-click the file, open Properties and tick Unblock if it appears. Then open it in Excel for Windows and choose Enable Content.
3. Type an NSE symbol, BSE code or company name in the yellow cell on the Cover sheet and pick Consolidated or Standalone.
4. Click the fetch button. The data download needs an internet connection and takes roughly 5 to 15 seconds.
5. Review the Assumptions sheet. Defaults come from the last three years, and any yellow cell can be overridden.
6. Switch the scenario on the Cover sheet. The statements, ratios and DCF recalculate.

Colour code: blue text is a hard-coded input or fetched data, black text is a formula, green text is a link to another sheet, and yellow cells are the ones you may edit.

## Berger Paints example

The valuation, assumptions and sensitivity table are in the PDF. Key choices:

- Cost of equity uses a 5-year daily regression beta
- Terminal growth of 5%, with return on new capital set to the forecast after-tax ROIC
- A reverse DCF shows what growth the market price implies

## Limitations

- Built for non-financial companies. Banks and NBFCs will load, but the EBITDA and working-capital logic is indicative only.
- The data fetch needs Excel for Windows. The model itself works elsewhere.
- Historical figures come from Screener.in public pages. Check material numbers against the annual reports.
- Some historical other liabilities and other current assets are balancing items derived from Screener totals.

## Disclaimer

This is a learning project, not investment advice. The views are my own.

## Author

Aarav Kapoor
