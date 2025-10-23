# 📊 Web3 Trading Behavior & Market Sentiment Analysis  

## 🧠 Project Overview  
This project analyzes the relationship between **trader behavior** (profitability, leverage, position size, and trade direction) and the **market sentiment** (Fear & Greed Index).  
The goal is to understand how emotions reflected in sentiment influence trading patterns and outcomes in the crypto market.

---

## 🗂️ Datasets  

### 1. **Historical Trading Data**  
**Source:** [Google Drive Link](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)  
**Description:**  
Contains information about trader activities including:  
- `timestamp` – Trade closing time  
- `Closed PnL` – Profit or loss on each trade  
- `Size USD` – Trade size in USD  
- `Side` – Buy/Sell direction  
- `Leverage`, `Start Position`, `Crossed`, `Coin`, and other metrics  

---

### 2. **Fear & Greed Index Data**  
**Source:** [Google Drive Link](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)  
**Description:**  
Provides daily sentiment of the crypto market including:  
- `Timestamp IST` – Date and time of the index  
- `Classification` – Sentiment label (Fear, Greed, Neutral)  
- `Value` – Numeric sentiment score  

---

## ⚙️ Data Preprocessing  

- Converted timestamps (`timestamp` & `Timestamp IST`) to date format  
- Merged both datasets on the `date` column  
- Cleaned missing values and ensured numerical types for key metrics  
- Filtered out invalid or incomplete sentiment records  

---

## 🔍 Exploratory Data Analysis (EDA)  

### 1. Profitability vs Sentiment  
- Analyzed average and distribution of `Closed PnL` under each sentiment (Fear, Neutral, Greed).  
- Visualized results using boxplots to capture variation in trader performance.  

### 2. Trading Volume by Sentiment  
- Aggregated total trade volume (`Size USD`) by sentiment category.  
- Used bar charts to identify risk appetite patterns during different market moods.  

### 3. Leverage & Risk Behavior  
- Compared average leverage and position size across sentiments.  
- Observed how traders take higher or lower risk in Fear vs Greed periods.  

### 4. Buy/Sell Direction Analysis  
- Counted and visualized trade directions (Buy/Sell) by sentiment.  
- Explored how sentiment affects bullish/bearish bias in trades.  

### 5. Coin-Level Insights  
- Identified most traded and profitable coins during each sentiment phase.  
- Showcased potential patterns for coin selection strategy.  

### 6. Time-Series Profitability Trends  
- Visualized average daily `Closed PnL` alongside sentiment value.  
- Examined profit fluctuations with changes in market sentiment.  

---

## 📈 Key Insights  

- **Fear phases** often lead to reduced trading volume and more conservative positions.  
- **Greed phases** correspond with higher leverage and risk-taking.  
- Profitability trends vary significantly between sentiment types.  
- Sentiment indicators can serve as early signals for shifts in trading behavior.  

---

## 🧩 Tools & Libraries Used  

- **Python**  
- **Pandas**, **NumPy** – Data cleaning & processing  
- **Matplotlib**, **Seaborn** – Data visualization  
- **Jupyter / Google Colab** – Interactive analysis environment  

---

## 💡 Conclusion  

Market sentiment plays a crucial role in shaping trader behavior.  
Integrating Fear & Greed sentiment data with trading activity helps identify patterns that can guide **data-driven trading strategies** and **risk management decisions**.  

---

## 📁 Folder Structure  

```
📂 ds_bhimashankar/ 
├── notebook_1.ipynb           # All work done in Google Colab                 
├── csv_files/                 # Store all CSVs or data outputs here.    
│   └── *.csv                  # Any intermediate or processed data files.     
├── outputs/                   # Store all visual outputs, graphs, or charts here.     
│   └── *.png / *.jpg          # Image results of EDA, charts, etc.     
├── ds_report.pdf              # Final summarized insights and explanations.    
└── README.md                  # (Optional but encouraged) Setup  instructions, notes.   
 
```

---

## ✍️ Author  

**👤 Bhimashankar Suksen Patil**  
📧 [bhima5136@gmail.com](mailto:bhima5136@gmail.com)  
📍 Mumbai, Maharashtra, India  
💼 Data Analyst | Data Science Enthusiast  

---

## ⭐ How to Use  

1. Download the datasets from the above Drive links.  
2. Open `notebook_1.ipynb` in Jupyter/Colab.  
3. Run all cells sequentially to reproduce the results.  
4. Review visualizations in the `outputs/plots/` folder.  

---

## 🧭 Future Improvements  

- Include live sentiment data using APIs  
- Extend analysis to multiple coins  
- Integrate machine learning models to predict profitability based on sentiment  

