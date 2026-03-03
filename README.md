# Risk-Adjusted Momentum (RAM)

A systematic framework for conditional crypto exposure designed to improve risk efficiency relative to passive BTC buy-and-hold.

📄 Full Research Paper (PDF):  
→ [Risk_Adjusted_Momentum_RAM.pdf](./Risk_Adjusted_Momentum_RAM.pdf)

---

## Objective

Bitcoin has delivered strong long-term returns but with extreme volatility and repeated deep drawdowns.

This research evaluates whether conditional exposure based on risk-adjusted momentum can improve the risk-adjusted profile of crypto investing relative to passive BTC buy-and-hold (BAH).

The emphasis of this work is methodological discipline rather than return maximization.

---

## Research Framework

The study follows a structured quantitative research protocol:

1. Define an economic objective  
2. Formulate explicit, testable hypotheses  
3. Construct a systematic signal  
4. Constrain parameter exploration  
5. Select from stability regions (not peak Sharpe)  
6. Validate on a fully independent out-of-sample period  

No parameters were modified after observing out-of-sample results.

---

## Strategy Overview

**Universe:**  
BTC, ETH, XRP, SOL, BNB  

**Signal:**  
Rolling return per unit of risk (Sharpe-like measure)

\[
RAM_{i,t} = \frac{R_{i,t-n:t}}{\sigma_{i,t-n:t}}
\]

**Logic:**  
- Long when |RAM| exceeds threshold  
- Otherwise neutral  
- Equal-weight across active assets  
- No short positions  
- Daily evaluation  

Both positive and extreme negative RAM signals were found to contain predictive information.

---

## Parameter Discipline

- Observation window: 5–20 days  
- Signal threshold: 0.10–0.40 (constrained grid)  
- 69 combinations evaluated  
- Selection based on stability across parameter regions  

A 50/50 combination of two adjacent stable parameter sets was used to reduce sensitivity.

---

## Results Summary

### Training Period (2021–2023)

| Metric | RAM Combo | BTC BAH |
|---------|-------------|------------|
| CAGR | 75% | 38% |
| Sharpe | 2.10 | 0.50 |
| Max DD | -16% | -124% |
| Correlation to BTC | 35% | — |

---

### Out-of-Sample Period (2024–2025)

| Metric | RAM Combo | BTC BAH |
|---------|-------------|------------|
| CAGR | 49% | 59% |
| Sharpe | 2.46 | 0.98 |
| Max DD | -10% | -37% |
| Correlation to BTC | 39% | — |

Although BTC generated higher absolute returns during the test period, RAM delivered materially lower volatility and drawdown while remaining invested only ~32% of the time.

---

## Key Findings

- Risk-adjusted momentum persists in crypto markets.  
- Extreme negative momentum often signals short-term reversal.  
- Conditional exposure reduces participation during high-volatility transitions.  
- Diversification across large-cap crypto reduces concentration risk.  
- Stability-region parameter selection improves generalization.

---

## Research Contribution

The primary contribution of this paper is methodological:

- Hypothesis-driven framework  
- Constrained parameter exploration  
- Stability-based selection  
- Clean train/test separation  
- Transparent reporting of limitations  

This work demonstrates a disciplined quantitative research process applied to a highly volatile asset class.

---
