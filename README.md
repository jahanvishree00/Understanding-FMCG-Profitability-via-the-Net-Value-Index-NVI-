# Understanding-FMCG-Profitability-via-the-Net-Value-Index-NVI-
I built this project to challenge a common assumption in the Fast-Moving Consumer Goods (FMCG) sector: does moving inventory faster and cutting costs always lead to higher profit margins?

# Why Marico and Dabur?
To examine how operational supply chain mechanics translate into bottom-line profitability, this project evaluated two of India’s most resilient, domestically anchored Fast-Moving Consumer Goods (FMCG) powerhouses: Marico Limited and Dabur India Limited.

Both enterprises operate at comparable financial scales (annual revenues oscillating between ₹7,000 Cr and ₹13,000 Cr across FY 2019–2025) and navigate identical macro headwinds—including rural demand cycles, crude-linked packaging spikes, agricultural inflation, and intense distribution competition

# Tools and Methods
1)Data Sources: Yahoo Finance, Screener.in, and company annual reports.

2)Analysis: Microsoft Excel (Min-Max scaling, Pearson correlation, linear regression).

3)Methodology: Tested heuristic industry-standard weightings against proportional correlation weighting to see which model actually predicted real-world margins.

# Methodology 
A frequent mistake in financial modeling is circularity—for example, using a financial output like gross margin to predict net margin. To keep this analysis strictly empirical, I built the NVI using only physical and operational input variables:

Inventory Turnover Ratio (ITR): Evaluates warehouse throughput and inventory velocity.

Operating Expense (Opex) Ratio: Evaluates overhead, logistics, and distribution cost efficiency.

Because you cannot simply add a turnover multiple to a percentage, I normalized these variables onto a uniform 0-100 scale using Min-Max scaling. Negative drivers, like Opex, were inverted so that a higher score consistently signifies better efficiency.

# Key Findings: The Tale of Two Supply Chains
1. Dabur: The Textbook Velocity Engine
Dabur's data validated the standard FMCG doctrine perfectly. Their operational profitability is overwhelmingly governed by speed-to-shelf.

Statistical Weights: 78% Inventory Turnover / 22% Opex Efficiency

Correlation to Profit: +0.79 (Strong Positive)

When Dabur moves its highly perishable food and personal care inventory out of warehouses faster, their margins expand linearly. Operating expenses matter, but inventory velocity is the undisputed engine of their business.

2. Marico: The Strategic Stockpiling Anomaly
Marico broke the fundamental model entirely, revealing a massive supply chain anomaly.

Statistical Weights: 50% Inverted Inventory Turnover / 50% Opex Efficiency

Correlation to Profit: +0.90+ (Near-Perfect Positive)

Initially, Marico's profit showed a severe negative correlation (-0.92) with inventory turnover. The data revealed that because Marico relies heavily on Copra (coconut) as a raw material, management intentionally stockpiles physical inventory when commodity prices crash. This tanks their turnover ratio in the short term but locks in bottom-cycle costs, driving massive margin expansion in subsequent quarters. Once the index was adjusted to treat lower turnover as a deliberate strategic buffer, the model perfectly predicted their profitability.
