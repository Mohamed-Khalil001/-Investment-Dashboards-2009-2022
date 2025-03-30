# ![image](https://github.com/user-attachments/assets/bde19d5e-1995-40c5-a1c8-af6889d25054) Investment Dashboard: A Power BI Analysis (2009-2022)

## 🌟 Project Overview
Welcome to **Investment Dashboards**, a comprehensive data analysis project that dives deep into the financial performance of major companies from 2009 to 2022. Using **Power BI**, I transformed raw Excel data into **4 interactive dashboards** to uncover market trends, financial metrics, and sector dominance. The project tells a compelling story of Wall Street's journey through economic crises, technological booms, and inflationary pressures.

This project showcases my skills in **data analysis**, **data visualization**, and **storytelling** while providing actionable insights for investors and analysts.

---

## 📂 Data Cleaning & Preprocessing

### ✨ Handling Missing Values
- **Statistical Imputation**: For missing financial metrics (e.g., ROE, Free Cash Flow), I applied **mean/median imputation** to maintain data integrity without skewing trends.
- **Categorical Handling**: Missing sector classifications were assigned based on similar companies.

### ⚡ Removing Bias: Dropping 2023 Data
- **Why?** Some companies had reported **2023 data**, while others hadn’t, creating an unfair advantage.
- **Solution**: Removed **2023 entirely** to ensure an equal comparison across all companies.
- **Impact**: This prevents misleading conclusions about performance disparities.

---

## 🔄 Measures & Calculations in Power BI
I created multiple **DAX Measures** to extract insights from raw data:

### 1. Market Performance Measures
- **Total Market Cap** = `SUM([Market Cap])` → Aggregates company values to assess sector dominance.
- **Volatility (Standard Deviation)** = `STDEV.P([Stock Price Change])` → Evaluates investment risk.
- **Market Share %** = `[Company Market Cap] / [Total Market Cap]` → Identifies industry leaders.

### 2. Profitability & Efficiency Measures
- **Return on Equity (ROE%)** = `[Net Income] / [Shareholder Equity]` → Measures company profitability.
- **Net Profit Margin (%)** = `[Net Income] / [Revenue]` → Evaluates operational efficiency.
- **EBITDA Growth %** = `([EBITDA] - PREVIOUSYEAR([EBITDA])) / PREVIOUSYEAR([EBITDA])` → Tracks profitability trends.

### 3. Sector Analysis Measures
- **Sector Contribution %** = `[Sector Revenue] / [Total Revenue]` → Highlights dominant industries.
- **Sector Volatility** = `STDEV.P([Stock Returns])` → Determines stability across industries.
- **Inflation Impact** = `[Sector Growth] - [Inflation Rate]` → Analyzes inflation-adjusted performance.

These measures helped shape the insights displayed in the dashboards, ensuring precise financial storytelling.

---

## 📂 Project Structure

The repository is organized as follows:
```
Investment-Dashboards/
│
├── data/
│   ├── investment_data.xlsx
│
├── powerbi/
│   ├── investment_report.pbix
│
├── screenshots/
│   ├── market_overview.png
│   ├── financial_performance.png
│   ├── sector_analysis.png
│   ├── final_story.png
│
├── story-insights/
│   ├── story.pdf
│   ├── insights_and_recommendations.pdf
```

---

## 📈 Dashboard Overview

The project consists of **4 interconnected dashboards**, each designed to provide specific insights into the investment landscape:

### 1. Market Overview
- **Purpose**: Highlights market trends, growth opportunities, and volatility.
- **Key Insights**:
  - 🌟 **Fastest-growing company**: NVDA (**96x growth** since 2009).
  - ⚠ **Most volatile company**: NVDA (**Standard Deviation: 150%**).
  - 🏦 **Top market cap**: AAPL (**$2.07T in 2022**).
  - 👑 **Dominant sector**: IT (**50% market share**).
  ![Market Overview](<https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/1ed76bb03a74bb812ad7895cbfdca236b5f6fc29/3-Dashboard%20Images/1-overview.png>)
### 2. Financial Performance
- **Purpose**: Analyzes financial health through key metrics like **ROE, ROA, and Free Cash Flow**.
- **Key Insights**:
  - 🏆 **ROE**: AAPL leads with **196.96%**.
  - 💰 **Free Cash Flow**: AAPL at **$99.8B**, followed by GOOG (**$71.2B**).
  - 📊 **Net Profit Margin**: MSFT (**36.69%**), NVDA (**36.23%**).
  - 📈 **Revenue Growth**: AMZN leads with **$513.98B** in 2022.
  ![Financial Performance ](<https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/1ed76bb03a74bb812ad7895cbfdca236b5f6fc29/3-Dashboard%20Images/2-Financial_performance.png>)

### 3. Sector Analysis
- **Purpose**: Compares **IT, LOGI, ELEC, FOOD, and BANK** sectors by profitability and stability.
- **Key Insights**:
  - ⚖️ **Most stable sector**: LOGI (**StdDev: 2.28**).
  - 💪 **Highest EBITDA**: IT (**$2.07683T**).
  - 📊 **Net Profit Margin by Sector**: IT (**27.73%**), ELEC (**24.47%**), LOGI (**-0.53%**).
  - 📉 **Inflation Trend**: Peaked at **8% in 2022**, impacting sectors like LOGI.
  ![Sector Analysis ](<https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/1ed76bb03a74bb812ad7895cbfdca236b5f6fc29/3-Dashboard%20Images/3-sector_analysis.PNG>)


### **4. Final Story**  
- **Purpose**: Summarizes the investment journey with actionable recommendations.  

  -📖 [**The Story**](https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/517102324c53c9c888831d81c7fa8eee2dd0bde3/4-Story%20_insights%20and%20Recommendations/Insights%20and%20Recommendation.pdf)  
  -🔍 [**Key Insights and Recommendations**](https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/517102324c53c9c888831d81c7fa8eee2dd0bde3/4-Story%20_insights%20and%20Recommendations/The_Story.pdf)  

   ![Final Story](https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/blob/517102324c53c9c888831d81c7fa8eee2dd0bde3/3-Dashboard%20Images/4-final_story.PNG)


---

## 🛠️ Tools Used
- **Power Query**: Data preparation & cleaning.
- **Power BI**: Data modeling & visualization.
- **DAX**: Created advanced measures.
- **Git & GitHub**: Version control & project hosting.

---

## 🎮 How to Use

1. **Explore the Dashboards Locally**:
   - Download the `investment_report.pbix` file from [<https://github.com/Mohamed-Khalil001/-Investment-Dashboards-2009-2022/tree/1ed76bb03a74bb812ad7895cbfdca236b5f6fc29/1-poject%20(pbx%20file)>].
   - Open it in [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) to interact with the dashboards.

2. **View the Live Dashboards**:
   - Access them here: [Power BI Report](https://app.powerbi.com/groups/me/reports/bd33330c-ad23-440b-9542-b1b76e9058e4?ctid=0ffeb7b8-177f-48b0-809f-2499efab9107).

3- **Download The Database and start your project**
   - Dowload: [Kaggle database](https://www.kaggle.com/datasets/rish59/financial-statements-of-major-companies2009-2023)

---

## 💌 Contact
- **LinkedIn**: [Mohamed Abdelfattah](https://www.linkedin.com/in/mohamed-abdelfattah-59035a353)
- **Email**: [muhammadabdelfattah177_sd@nsst.bsu.edu.eg]

---

🌟 **If you find this project useful, give it a star!** 💫

