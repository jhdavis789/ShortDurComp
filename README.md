# ShortDurComp

Short-Duration ETF competitor dashboard — 19 funds across iShares, PIMCO, and Franklin Templeton.

Built for a PM designing a competing short / ultra-short-duration ETF whose compensation is benchmarked to 3Y relative outperformance. Seven tabs: Landscape, Risk Matrix, Stress, Historical Pain, Drill-down, Yield Decomp, Factor Betas.

- Risk Matrix uses Basel III LCR HQLA haircuts for the Liquidity axis
- Stress shown both model-based (duration × shock) and realized (factor-β × historical shock)
- Drawdowns back to 1987 (FISAX via Franklin Templeton monthly blend)
- Exposure similarity via cosine on sector / rating / maturity / factor-β / combined vectors
- All numbers computed in `short_duration_risk.py`; dashboard renders only

Source: <https://github.com/jhdavis789/bdc-portfolio-dashboard/tree/newpull-soi-pipeline/research/PIMCO>
