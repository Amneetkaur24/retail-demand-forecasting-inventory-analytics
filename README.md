📊 Retail Demand Forecasting & Inventory Optimization

Demand Forecasting | Inventory Policy Design | Promotion Impact Analysis

📌 Project Overview

Retail businesses frequently lose revenue due to stockouts, overstocking, and poorly timed promotions. Without reliable demand forecasting, inventory decisions become reactive and inefficient.

This project builds an end-to-end analytics framework that forecasts demand, identifies key demand drivers, and translates predictions into inventory policies and operational decisions.

The solution integrates machine learning forecasting with inventory optimization to support data-driven retail planning.

🎯 Business Problem

Retail decision makers must answer three critical questions:

• What will demand look like in the future?
• What factors actually drive demand?
• How much inventory is needed to avoid stockouts while controlling holding costs?

Traditional forecasting models often ignore operational constraints such as lead times, safety stock, and promotion-driven demand spikes.

This project addresses these gaps by connecting demand forecasting with inventory policy simulation.

🚀 Solution

The project delivers a complete analytics pipeline that:

• Forecasts product demand using machine learning models
• Identifies key drivers of demand using model explainability
• Quantifies the impact of pricing and promotions
• Calculates safety stock and reorder points
• Simulates stockout vs holding cost tradeoffs
• Presents insights via an interactive dashboard

📊 Dashboard Preview
<img width="859" height="600" alt="image" src="https://github.com/user-attachments/assets/418b9633-9082-41b7-9192-3fd1e944ca50" />

🔗 Live Dashboard:
https://retail-demand-inventory-dashboard-cqktcqkohdrytlemhh6d8y.streamlit.app/

🧠 Key Analytics Components
1️⃣ Demand Pattern Analysis

Analyzed sales patterns across:

• product categories
• promotions
• weekdays and seasons
• sales channels

This revealed structural demand differences across categories.

2️⃣ Baseline Time-Series Forecasting

A 3-month rolling average forecast was built to establish a baseline model.

Purpose:

• capture seasonality
• identify long-term trends
• create a benchmark for ML models

3️⃣ Machine Learning Demand Forecasting

Demand was predicted using Random Forest and Gradient Boosting models.

Target Variable

Quantity Sold (units)

Features

• Price per unit
• Promotion intensity
• Stock availability
• Seasonality
• Month and weekday
• Product category

Model Performance

MAE ≈ 2.39 units

This indicates the model predicts demand within roughly 2–3 units per transaction.

4️⃣ Model Explainability

Feature importance analysis identified the primary drivers of demand:

1️⃣ Stock availability
2️⃣ Product price
3️⃣ Promotions
4️⃣ Category effects
5️⃣ Weekday patterns

This ensures the model is interpretable and business-aligned.

5️⃣ Inventory Policy Optimization

Forecast outputs were converted into operational inventory decisions.

Key calculations include:

Safety Stock

Protects against forecast errors and demand spikes.

Reorder Point (ROP)

ROP = (Average Daily Demand × Lead Time) + Safety Stock

Ensures stock replenishment before shortages occur.

6️⃣ Demand Scenario Simulation

To test inventory robustness, demand shocks were simulated:

• Normal demand
• Promotional demand (+30%)
• Surge demand (+50%)

This stress testing helps identify categories vulnerable to stockouts.

📈 Key Business Insights

• Stock availability is the strongest driver of realized sales

Demand cannot be fulfilled if inventory is insufficient.

• Promotions increase demand only when inventory is available

Discount campaigns without stock preparation create stockouts.

• Forecast accuracy varies across categories

Some categories require higher safety stock buffers.

• Inventory risk depends on demand variability

High variability categories require more conservative inventory policies.

💼 Business Recommendations
Inventory Strategy

Maintain minimum stock thresholds for high-demand categories to prevent lost sales.

Promotion Planning

Promotions should be coordinated with inventory availability to avoid demand spikes causing stockouts.

Pricing Strategy

Price-sensitive categories should use dynamic pricing strategies rather than uniform price changes.

Category-Specific Policies

Different categories require different strategies:

• fast-moving goods → higher replenishment frequency
• premium goods → tighter inventory control

🛠 Tools & Technologies

Python
Pandas
NumPy
Scikit-learn
Matplotlib / Seaborn
Streamlit
GitHub

⚠️ Assumptions

• Lead time assumed constant
• Inventory review occurs daily
• Demand variability estimated using historical data
• Forecast errors assumed unavoidable

These assumptions approximate typical retail inventory operations.

🚀 Future Enhancements

• SHAP-based explainability
• Advanced time-series forecasting (Prophet / XGBoost)
• Dynamic pricing simulation
• Multi-warehouse inventory planning

👤 Author
Amneet Kaur
Data Analyst | Retail Analytics | Inventory Optimization
📍 Canada
