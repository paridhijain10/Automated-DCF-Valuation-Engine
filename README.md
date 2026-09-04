# Automated DCF Valuation Engine

A Python-based Discounted Cash Flow (DCF) valuation model for Apple Inc. (AAPL).

## Project Overview

This project estimates the intrinsic value of a company using a five-year Free Cash Flow to the Firm (FCFF) DCF model.

The model retrieves historical financial data, forecasts future cash flows, calculates WACC, estimates terminal value, and converts enterprise value into an implied equity value and share price.

## Key Features

- Historical financial statement analysis
- Revenue and EBIT analysis
- Free Cash Flow to the Firm (FCFF) calculation
- Five-year financial forecasting
- WACC calculation using CAPM
- Terminal value using the Gordon Growth Model
- Enterprise Value to Equity Value bridge
- Implied share price calculation
- WACC vs. terminal growth sensitivity analysis
- Bear, Base and Bull scenario analysis
- Financial data visualization

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- yfinance
- Google Colab

## Valuation Framework

Revenue → EBIT → NOPAT → FCFF → WACC → Enterprise Value → Equity Value → Implied Share Price

### Key Formulas

**FCFF**

FCFF = NOPAT + D&A − CapEx − Change in NWC

**Terminal Value**

Terminal Value = Terminal Year FCFF / (WACC − Terminal Growth Rate)

**Enterprise Value**

Enterprise Value = PV of Forecast FCFF + PV of Terminal Value

**Equity Value**

Equity Value = Enterprise Value − Debt + Cash

## Key Results

The base-case model produced an estimated intrinsic value of approximately **$111 per AAPL share**, compared with a market price of approximately **$328 per share at the time of analysis**.

Scenario analysis produced an approximate valuation range of:

- Bear Case: **$71/share**
- Base Case: **$111/share**
- Bull Case: **$167/share**

The model therefore indicates that the market price was substantially above the estimated intrinsic value under the selected assumptions.

## Important Note

This project is for educational and portfolio purposes and does not constitute investment advice.

DCF valuations are highly sensitive to assumptions including revenue growth, operating margins, WACC and terminal growth. The results should therefore be interpreted as an analytical valuation range rather than a precise price target.

## Project Structure

```text
Automated-DCF-Valuation-Engine/
│
├── DCF_Valuation_Engine.ipynb
└── README.md
