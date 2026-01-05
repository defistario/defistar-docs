Methodology
Transparency in DeFi Data Analytics

DeFiStar.io is built on the principle that accurate DeFi analytics must be derived directly from the blockchain, not from cached or abstracted third-party data. This document outlines, at a high level, how our data is sourced, processed, and transformed into meaningful yield and risk insights.

1. Data Sourcing & On-Chain Integrity
Direct Blockchain Access

DeFiStar does not rely on third-party aggregators or intermediary APIs. Instead, we perform direct Remote Procedure Calls (RPC) to blockchain nodes across more than nine supported networks.

This approach ensures that all displayed metrics — including yield and Total Value Locked (TVL) — are:

Not cached beyond design
Not delayed
Directly verifiable on-chain
Direct Smart Contract Querying

Using the eth_call method, DeFiStar.io queries protocol smart contracts directly to retrieve raw hexadecimal state data. This data is then decoded and normalised into usable financial metrics by our internal engine.
For example, liquidity data for Compound V3 is derived by querying the protocol’s core contract and decoding the returned values rather than relying on off-chain summaries.
This ensures the platform reflects the true on-chain state, exactly as protocols themselves see it.

2. Analytical Calculations

Once the raw blockchain state has been captured, DeFiStar.io’s analytical modules process this data into higher-level indicators designed to assess yield sustainability and market conditions.

Examples include but not limited to:

Money Flow Velocity
Money Flow Velocity measures capital movement by comparing 24-hour TVL changes against a 7-day rolling historical average. This helps distinguish organic capital flows from short-term or incentive-driven spikes.

DeFi Base Rate
The DeFi Base Rate represents a “risk-free” reference yield. It is calculated as a TVL-weighted average yield across blue-chip lending protocols such as Aave, Compound, and Spark. This provides a baseline against which higher-risk yields can be evaluated.

Utilisation Stress
Utilisation Stress is calculated as:
Total Borrowed / Total Supplied
Utilisation ratios exceeding 90% indicate liquidity strain and trigger immediate safety warnings, as high utilisation increases withdrawal and liquidation risk.

Market Sentiment
Market sentiment is derived using Least Squares Linear Regression applied to rolling 48-hour data snapshots. This allows us to estimate short-term market direction and identify accelerating or decelerating trends in lending demand.

3. Risk Radar & Safety Score

Protocol safety is assessed through a combination of automated audits and historical analysis. The Safety Score (0–100) is calculated using a weighted model across three core dimensions:

Component	Weight	Factors Assessed
Asset Integrity	40%	Stablecoin peg history and collateral quality
Protocol History	40%	Time since launch (Lindy Effect) and audit track record
Network Resilience	20%	Chain decentralisation and base-layer security

Penalty Adjustments
Score deductions are applied for:
TVL below $1 million
Abrupt utilisation “kinks”
Yield anomalies where APY exceeds 15% without clear incentive justification
These penalties are designed to highlight structural risk, not short-term opportunity.

4. Stablecoin & Oracle Verification

DeFiStar.io does not rely solely on displayed prices. Stablecoin health is verified through on-chain price oracles, queried directly within the same environment used by lending protocols themselves.
This approach allows DeFiStar to detect:
Early de-pegging events
Oracle-level price deviations
Risk conditions that precede protocol liquidations

By monitoring oracle data directly, users receive warnings at the same decision layer used by smart contracts, not at a delayed market-price level.

5. Methodology Principles

On-chain first — data is sourced where it originates
No aggregation bias — no third-party abstraction layers
Risk-aware, not yield-chasing — sustainability over headline returns
Transparency over complexity — clear metrics users can reason about

📜 License

Documentation in this repository is licensed under: Creative Commons Attribution 4.0 International (CC BY 4.0)
You are free to: Share Adapt Build upon this work With appropriate attribution to DeFiStar.io 🤝 Contributions & Feedback
Feedback, issues, and suggestions are welcome. This repository exists to support: Ethereum researchers DeFi builders Public goods initiatives

🔗 Links 🌐 Website: https://defistar.io 🐦 X: https://x.com/moonitooki

📣 Disclaimer

Defistar.io provides informational analytics and data services only. We are not authorised or regulated by the Financial Conduct Authority (FCA). We do not offer, facilitate, or provide any financial services or products, including cryptocurrencies, digital assets, or derived products. Content on defistar.io does not constitute financial advice. DeFiStar.io is an independent data utility. We do not accept listing fees, we do not have an affiliate relationship with protocols, and we do not sell financial products. Our rankings are 100% algorithmic based on on-chain liquidity and smart contract data. By accessing or using our website, you agree to be bound by our Terms of Service and acknowledge our Risk Disclosures.

Nothing here or on our website constitutes financial advice. Full project terms at https://defistar.io/terms.php
