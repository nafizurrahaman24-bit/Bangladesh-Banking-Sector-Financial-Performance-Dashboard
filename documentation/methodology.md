# Methodology

## 1. Study Scope

This project compares 11 selected commercial banks in Bangladesh over 2021–2025.

The sample contains 10 private commercial banks and 1 government-owned commercial bank.

The results represent a comparative assessment of the selected sample, not the entire Bangladesh banking sector.

## 2. Unit of Analysis

The primary observation unit is the **bank-year**.

With 11 banks observed annually from 2021 through 2025:

**11 × 5 = 55 bank-year observations**

This assumes the final dataset contains one valid observation for every bank-year combination.

## 3. Average Performance

The dashboard focuses on **average annual reported bank-level performance over the examined period**.

For example, average ROA is the mean of a bank's annual ROA observations across 2021–2025.

These averages describe typical performance over the study period rather than latest-year performance alone.

Power BI's standard **Average** aggregation is used where appropriate. Custom DAX is used for ranking, dynamic selection, and other analytical logic where required.

## 4. Financial Dimensions

- **Profitability:** ROA, ROE, NIM, Net Income, EPS
- **Asset Quality:** NPL Ratio, Total NPL, Loan-Loss Provision
- **Capital:** CAR, Tier-1 Capital Ratio
- **Liquidity & Efficiency:** LDR, CIR
- **Market Performance:** P/B Ratio, EPS, Market Value

## 5. Composite Ranking

The overall ranking uses an **equal-weighted average-rank approach** across:

1. ROA
2. ROE
3. NPL Ratio
4. CAR
5. CIR

| Indicator | Preferred Direction |
|---|---|
| ROA | Higher |
| ROE | Higher |
| NPL Ratio | Lower |
| CAR | Higher |
| CIR | Lower |

Each bank receives an indicator-level rank. The five ranks are then averaged:

**Overall Average Rank = Mean of ROA Rank, ROE Rank, NPL Rank, CAR Rank, and CIR Rank**

The final ranking is based on the Overall Average Rank:

**Lower Overall Average Rank = Stronger comparative performance**

Each selected indicator receives equal weight.

## 6. LDR Treatment

LDR is treated as a liquidity indicator but is excluded from the composite ranking because higher or lower LDR is not inherently better without a justified benchmark or optimal range.

## 7. Missing Values

Missing observations should not be treated as zero. Where a reported value is unavailable, it remains missing and is excluded from an average calculated over available valid observations.

## 8. Interpretation of Relationships

The analysis is descriptive and comparative. Observed relationships, such as the tendency for lower CIR to coincide with stronger ROA, should not be interpreted as causal without additional statistical testing.

## 9. Limitations

- The sample contains 11 selected banks, not the full banking sector.
- The study covers 2021–2025.
- Averages may hide year-specific shocks.
- Reporting differences may affect comparability.
- The composite ranking depends on the selected indicators and equal weighting.
- LDR is excluded from the composite because its optimal direction is context-dependent.
- The analysis does not establish causal relationships.
