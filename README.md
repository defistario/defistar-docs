# defistar-docs
DeFiStar.io Documentation & Methodology
Transparent On-Chain Yield & Risk Analytics for DeFi

📌 Overview

DeFiStar.io is an independent DeFi analytics platform focused on stablecoin lending yields and risk transparency, built using direct on-chain blockchain RPC data avoiding third-party aggregators.

This repository will contain documentation, methodology, and reference material describing how DeFiStar.io sources, normalises, and analyses on-chain data to produce reliable yield and risk insights for the Ethereum ecosystem.

🔗 Live platform: https://defistar.io

🎯 Mission

Our mission is to make DeFi safer, more transparent, and easier to understand, especially for users seeking information about stablecoin yields.

We believe:

On-chain data should be sourced directly from the blockchain

Analytics tools should be neutral and unbiased

Users deserve clear risk context, not just headline APYs

🔍 What Makes DeFiStar.io different

Analytics platforms tend to rely on third-party aggregators and APIs, which can:
Introduce latency or inaccuracies

Apply opaque filtering or assumptions

Create hidden dependencies

DeFiStar.io bypasses aggregators entirely.

Key Principles

✅ Direct RPC calls to blockchain nodes
✅ Data pulled straight from protocol smart contracts
✅ Hourly updates with minimal latency
✅ No paid listings, no affiliate links
✅ Independent ranking and safety metrics

This ensures verifiable, on-chain truth.

🧠 What This Repository Contains

This repository is intentionally focused on documentation and public-good artifacts, not production infrastructure.

To be included:
📄 Platform architecture overview
📊 Data sourcing & normalisation methodology
🧮 Yield calculation explanations
🛡️ Risk & safety scoring concepts (high-level)
🧪 Reference examples (non-production)
🗺️ Roadmap & planned public deliverables

Not included:

❌ Production backend code
❌ Private infrastructure
❌ Proprietary algorithms

This balance allows transparency without compromising security or sustainability.

🏗️ Architecture Overview (High Level)

Blockchain RPC Nodes
Ethereum + major L2s
Protocol Smart Contracts
Aave V3, Compound V3, Morpho, Spark, etc.

On-Chain Data Extraction
Interest rates, utilisation, liquidity, TVL

Normalisation Layer
Standardized yield and risk metrics

Analytics Engine
Stability, turbulence, stress indicators

User Interface
Simple, readable dashboards

All core metrics are derived from verifiable on-chain sources.

📈 Yield Metrics Explained

DeFiStar.io tracks:
Current APY
Rolling average APY
Utilisation ratios
Liquidity depth
Historical stability indicators
Yields are calculated directly from protocol parameters and contract state — not estimated from external feeds.

🛡️ Risk & Safety Metrics (Conceptual)

Risk indicators are designed to help users assess sustainability, not to predict price movements.

High-level inputs include:
Liquidity availability
Utilisation volatility
Rate change frequency
Historical reliability patterns

⚠️ Scores are informational, not financial advice.
🌍 Public Good Commitment

DeFiStar.io is built as neutral infrastructure for the Ethereum ecosystem and wider DeFi ecosystems.

Core analytics remain free and publicly accessible
Focus on education, safety, and transparency

Designed to support researchers, DAOs, and users
Expand public knowledge
Improve data transparency
Reduce information asymmetry in DeFi

🧩 Sustainability

The platform follows a freemium model:
Free access to core dashboards
Optional premium features for advanced users will come in due course
No extraction from protocols or users
This ensures long-term maintenance without compromising independence.

🛠️ Reference Examples

Where appropriate, we may publish:
Example RPC queries
ABI decoding references
Sample yield calculation logic
All examples are educational only and not production-ready.

🗺️ Roadmap (Public Deliverables)

Expanded methodology documentation
Historical data access for research
Alerting & monitoring concepts
Public API design (rate-limited)

📜 License

Documentation in this repository is licensed under:
Creative Commons Attribution 4.0 International (CC BY 4.0)

You are free to:
Share
Adapt
Build upon this work
With appropriate attribution to DeFiStar.io
🤝 Contributions & Feedback

Feedback, issues, and suggestions are welcome.
This repository exists to support:
Ethereum researchers
DeFi builders
Public goods initiatives

🔗 Links
🌐 Website: https://defistar.io
🐦 Twitter/X: https://x.com/moonitooki

📣 Disclaimer

Defistar.io provides informational analytics and data services only. We are not authorised or regulated by the Financial Conduct Authority (FCA). We do not offer, facilitate, or provide any financial services or products, including cryptocurrencies, digital assets, or derived products. Content on defistar.io does not constitute financial advice.
DeFiStar.io is an independent data utility. We do not accept listing fees, we do not have an affiliate relationship with protocols, and we do not sell financial products. Our rankings are 100% algorithmic based on on-chain liquidity and smart contract data.
By accessing or using our website, you agree to be bound by our Terms of Service and acknowledge our Risk Disclosures.

Nothing here or on our website constitutes financial advice. Full project terms at https://defistar.io/terms.php
