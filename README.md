# JSE Equity Portfolio: A Top-Down Investment Framework

A stock-screening and valuation workbook I use to build and manage a real-money portfolio of JSE-listed shares. It works from the top down: start with the South African economy, decide which sectors to own, screen the companies in those sectors on quality, then value the survivors with a discounted cash flow model before buying.

> GitHub can't preview Excel files. To explore the workbook, click the `.xlsx` file in this repo, then the download button, and open it in Excel.

## How the framework works

### 1. Macro view and sector selection

Sector weights come from where the economy is in its cycle, read from three indicators:

- **Producer Price Index (PPI)** for input-cost pressure and pricing power
- **The yield curve** for the interest-rate outlook and recession risk
- **Business confidence** for the direction of corporate activity

The current allocation:

| Sector | Weight |
| --- | --- |
| Mining | 65% |
| Retail | 20% |
| Agriculture & services | 15% |

### 2. Quality screen

Each candidate (12+ companies so far) has to pass three financial-strength tests before it is valued:

| Metric | Threshold | Why it matters |
| --- | --- | --- |
| Return on equity (ROE) | > 15% | The business earns well on shareholders' capital |
| Debt-to-equity (D/E) | < 0.5 | Low leverage, so less exposed to rate rises and downturns |
| Interest coverage | > 5x | Earnings comfortably cover interest payments |

### 3. Valuation: two-stage FCFE DCF

Companies that pass the screen are valued with a two-stage free cash flow to equity (FCFE) model, following Aswath Damodaran's approach:

- **Stage 1:** explicit forecasts of free cash flow to equity over the high-growth period
- **Stage 2:** a terminal value with deliberately conservative assumptions: long-run growth of 3–4%, and excess returns that fade towards the cost of equity rather than lasting forever

The intrinsic value per share is then compared with the market price to find undervalued, high-conviction holdings.

### 4. Portfolio management and risk controls

- **Monthly DCA:** a fixed amount is invested each month rather than timing the market
- **Sector caps** keep any one sector from drifting too far past its target weight
- **A watchlist** of companies that pass the screen but aren't yet cheap enough
- **Ongoing review** through financial statement analysis, cycle positioning and adjustments for currency risk, which matters for rand-exposed and dollar-earning businesses alike

## Example holdings

Names that came through the screen and valuation as high-conviction picks include:

| Ticker | Company |
| --- | --- |
| ANG | AngloGold Ashanti |
| HAR | Harmony Gold Mining |
| AVI | AVI Limited |
| KST | PSG Financial Services |

## Results

The live portfolio is up **+4.4% (unrealised)** at the time of writing, built through monthly DCA.

## Tools

Microsoft Excel.

## Author

**Lanet Ndebe**, BSc Honours in Computer Science student at the University of the Witwatersrand, with a BSc in Computer Science and Finance.

- GitHub: [2626245](https://github.com/2626245)
- LinkedIn: [lanet-ndebe](https://www.linkedin.com/in/lanet-ndebe-7a57b7298)
- Email: lanetndebe@gmail.com

## Disclaimer

This is a personal project for learning and documenting my own process. It is not investment advice. Do your own research before buying any security. The data and information used was gathered on December 2025 .
