Retail Demand Forecasting & Inventory Optimization Dashboard



**Business Problem**
Retail businesses frequently lose revenue due to stockouts and overstocking.
This project uses historical sales data to forecast demand, assess promotion impact, and generate data-driven inventory recommendations.



**Solution**
This project builds an end-to-end analytics solution that:
• Analyzes demand patterns and seasonality
• Forecasts product demand
• Identifies key demand drivers
• Calculates safety stock and reorder points
• Simulates stockout vs holding cost scenarios
• Presents insights via an interactive Streamlit dashboard



**Live Demo**
Live Dashboard:
https://retail-demand-inventory-dashboard-cqktcqkohdrytlemhh6d8y.streamlit.app/
<img width="859" height="600" alt="image" src="https://github.com/user-attachments/assets/418b9633-9082-41b7-9192-3fd1e944ca50" />



**Tech Stack**
Python, Pandas, NumPy  
Matplotlib, Seaborn  
Scikit-learn  
Streamlit  
GitHub




**Key Business Insights**
• Stock availability is the strongest driver of realized sales
• Promotions increase demand only when inventory is sufficient
• Holding moderate safety stock is cheaper than stockout losses
• Inventory risk depends on variability, not just sales volume



**Project Structure**
├── data/
│   ├── cleaned_BrightMart_retail_dataset.csv
│   ├── inventory_policy.csv
│   ├── feature_importance.csv
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── EDA_Feature_Engineering.ipynb
│   ├── Forecasting_Model.ipynb
│   ├── Inventory_Optimization.ipynb
├── app.py
├── requirements.txt
├── README.md



**Future Improvements**
• SHAP-based explainability
• Product-level forecasting
• Confidence intervals for demand
• Multi-store inventory optimization
