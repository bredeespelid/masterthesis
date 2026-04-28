# Foundation Models for Time-Series Forecasting — EUR/NOK

A single-page GitHub Pages site summarising the master's thesis "Foundation Models for Time-Series Forecasting: Evidence from the EUR/NOK Exchange Rate" by Erlend Rake Ellingsen & Brede Espelid (NHH, 2025).

## Suggested repo names

- **`eurnok-foundation-models`** — descriptive, technical
- **`thesis-eurnok`** — short and clean
- **`nhh-thesis-foundation-models`** — institution-prefixed

I'd go with `eurnok-foundation-models`. URL: `https://bredeespelid.github.io/eurnok-foundation-models/`

## Deploy to GitHub Pages

1. Create a new public repo with the chosen name.
2. Rename `thesis-index.html` → `index.html` and push it to the root.
3. Optionally add the thesis PDF as `masterthesis.pdf` and link to it from the page.
4. Settings → Pages → Branch: `main` / `(root)`.
5. Wait ~30 seconds; live at `https://bredeespelid.github.io/eurnok-foundation-models/`.

## Add to your CV

```latex
\resumeProjectHeading
  {\textbf{Foundation Models for Time-Series Forecasting — EUR/NOK} $|$ \emph{Master's Thesis · NHH} {\href{https://bredeespelid.github.io/eurnok-foundation-models/}{\color{blue}Findings}} {\href{https://github.com/bredeespelid/eurnok-foundation-models/blob/main/masterthesis.pdf}{\color{blue}PDF}}}{}
  \resumeItemListStart
    \resumeItem{Tested whether transformer-based foundation models (Google TimesFM, Amazon Chronos2) can beat a driftless random walk and traditional benchmarks (VAR/VARX, XGBoost) at forecasting EUR/NOK at 1- and 3-month horizons.}
    \resumeItem{Chronos2 with cross-currency finetuning and a compact covariate set (VIX, S\&P 500, real exchange rate) significantly beats the random walk at the quarterly horizon (RMSE 0.1971 vs. 0.2127, Diebold--Mariano p=0.0230).}
    \resumeItem{Showed that information-set design matters more than model size: small, economically motivated covariates outperform broad macro kitchen-sink inputs.}
  \resumeItemListEnd
```

## Editing the page

Single `index.html` with inline CSS, no build step. Same design language as the operations-platform overview so the two sites feel like a coherent portfolio.
