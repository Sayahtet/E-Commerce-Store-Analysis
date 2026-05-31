
## Dataset

The dataset used is the classic **Superstore Sales Dataset**, containing order-level transactions from a fictitious retail chain. Key attributes include:
- Order & shipping dates  
- Product categories and sub‑categories  
- Sales, quantity, profit, and returns  
- Customer segments, regions, states, and cities  
- Payment methods  

*Note: The dataset is not included in this repository due to licensing/size constraints but can be obtained from [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) or similar sources.*

## Analytical Approach

The analysis follows a structured workflow:

1. **Data Cleaning & Preparation**  
   - Converted date columns to datetime format.  
   - Removed irrelevant columns (`ind1`, `ind2`).  
   - Verified data types and missing values.

2. **Key Performance Indicators (KPIs)**  
   - Total Sales, Total Profit, Total Quantity, Average Order Value, Profit Margin.

3. **Product‑Level Analysis**  
   - Sales and profit by Category and Sub‑Category.  
   - Identification of top/bottom performing products.

4. **Geographic & Customer Analysis**  
   - Regional and state‑wise profit/loss.  
   - Top cities and customer segments.  
   - Customer ordering frequency and profitability.

5. **Temporal Analysis**  
   - Monthly, quarterly, and period‑over‑period sales trends.  
   - Seasonal pattern detection.

## Key Findings & Business Insights

### 🏆 Top Performers
- **Category**: Technology generates the highest profit margin (~19%) and 51.6% of total profit.  
- **Sub‑Category**: Copiers are the most profitable; Phones lead in sales volume.  
- **Region**: West region dominates both sales (>30% share) and profit.  
- **State**: California and New York are top‑2 profit contributors.

### ⚠️ Areas of Concern
- **Sub‑categories**: Tables, Bookcases, and Supplies operate at a loss.  
- **States**: Texas, Illinois, Ohio, and Pennsylvania show significant losses.  
- **Seasonality**: Sales consistently dip in Q3 (September) and rise sharply in Q4 (November–December).

### 👥 Customer Insights
- **Consumer segment** accounts for 47% of total profit – primary target.  
- **Top customers** by sales and profit are identified; repeat purchase behavior analyzed.

### 📈 Strategic Recommendations
- Focus marketing and inventory on Technology products and the West region.  
- Investigate and remedy losses in Texas and underperforming sub‑categories.  
- Leverage Q4 peak season with promotions; plan for Q3 slowdown.  
- Build loyalty programs for high‑value customers (e.g., Caroline Jumper, Karen Ferguson).

## Visualizations

The notebook includes the following visual outputs:
- Bar charts (top products, states, customers)  
- Pie charts (profit/sales distribution by category, region, segment)  
- Line plots (monthly and quarterly sales/profit trends)  
- Horizontal bar charts (profit/loss by sub‑category)

## Power BI Dashboard Preview

An interactive **Power BI dashboard** was developed to complement the Python analysis, enabling dynamic filtering and real-time exploration of key metrics.

<img width="1789" height="771" alt="Screenshot 2026-05-31 213235" src="https://github.com/user-attachments/assets/cd355887-3646-4c43-8409-5a81079b5a9f" />
<img width="1826" height="872" alt="Screenshot 2026-05-31 213208" src="https://github.com/user-attachments/assets/fbf87ffd-e216-4987-be12-568e5297ba22" />
<img width="1552" height="728" alt="Screenshot 2026-05-31 214106" src="https://github.com/user-attachments/assets/97dc7a2a-1ee8-4cb7-82ef-083c3daf5ea8" />

This is my Power Bi Dashboard Link > https://app.powerbi.com/reportEmbed?reportId=34257c22-50e7-46c1-b1ee-e58fb0401f14&autoAuth=true&ctid=5aaf7eaa-31b7-4ea1-9318-274c220a2512&actionBarEnabled=true


*The dashboard includes:*
- KPI cards (Total Sales, Profit, Quantity)
- Sales and profit trends over time
- Geo‑mapping of profit by state
- Product category and segment breakdowns
## Requirements & Reproduction

To replicate this analysis, ensure the following Python packages are installed:

```bash
pip install pandas numpy matplotlib seaborn
