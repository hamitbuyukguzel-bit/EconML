# EconML: AI-Driven Dynamic Pricing & Revenue Optimization

A data science project exploring the intersection of **Microeconomics**, **Digital Marketing Strategy**, and **Machine Learning**. This tool determines the optimal pricing strategy to maximize revenue by modeling the Price Elasticity of Demand.

## 🎯 Objective
In the digital economy, pricing is not static. The goal of this project is to move beyond simple "Cost-Plus" pricing and utilize **predictive modeling** to find the price point that balances trade-offs between profit margins and sales volume.

## 🧠 Theoretical Background
The core logic relies on the economic concept of **Price Elasticity of Demand ($E_d$)**.
* **Elastic Demand:** Small price changes cause large demand shifts.
* **Inelastic Demand:** Demand remains stable despite price changes.
* **Optimization Goal:** Find the Price ($P$) where the first derivative of the Revenue function is zero ($R' = 0$).

## ⚙️ How It Works (The Algorithm)
1.  **Data Ingestion:** Takes historical sales data (Price vs. Quantity).
2.  **Demand Modeling:** Uses **Polynomial Regression** (Degree 2) to fit a non-linear demand curve, capturing real-world consumer behavior saturation.
3.  **Revenue Simulation:** Calculates projected revenue for a continuous range of potential prices ($Revenue = Price \times PredictedDemand$).
4.  **Optimization:** Identifies the global maximum of the revenue function to recommend the specific "Optimal Price".

## 🛠 Tech Stack
* **Python:** Core logic.
* **Scikit-Learn:** Polynomial Regression implementation.
* **Streamlit:** Interactive web dashboard.
* **Matplotlib & Seaborn:** Economic visualization (Revenue curves).

## 🚀 Installation & Usage

1.  Clone the repo:
    ```bash
    git clone [https://github.com/hamitbuyukguzel-bit/econml-pricing-optimizer.git](https://github.com/hamitbuyukguzel-bit/econml-pricing-optimizer.git)
    ```
2.  Install requirements:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the app:
    ```bash
    streamlit run app.py
    ```

## 📈 Future Work for PhD Research
This project serves as a baseline. Future iterations could include:
* **Competitor Analysis:** Incorporating competitor prices as external regressors.
* **Seasonality:** Using Time-Series Analysis (ARIMA/Prophet) for dynamic pricing over time.
* **Customer Segmentation:** Clustering users to offer personalized pricing.

---
