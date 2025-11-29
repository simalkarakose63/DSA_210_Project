#  COVID-19 and the Rise of E-Commerce in Turkey (2018–2025)

##  Introduction
This project explores how Turkey’s e-commerce market evolved before, during, and after the COVID-19 pandemic. The pandemic created one of the most rapid transitions to online shopping in modern history as lockdowns and restrictions forced consumers and businesses to shift to digital platforms. By analyzing official national datasets from 2018 to 2025, this project aims to understand whether the surge in e-commerce during COVID-19 was a short-term effect or a lasting structural change in Turkey’s retail landscape.

##  1. Motivation
COVID-19 dramatically reshaped global consumer behavior. In Turkey, the e-commerce sector grew at record speed as households adopted digital shopping out of necessity. As restrictions were lifted, an important question emerged:

> Has the shift toward online retail remained permanent, or did consumer habits revert to traditional physical shopping?

Understanding this transformation is crucial for analyzing Turkey’s economic digitalization, business strategies, and long-term consumer adaptation. This project seeks to provide a data-driven overview of how the pandemic accelerated digital transformation and changed the retail structure of Turkey’s economy.

##  2. Research Questions
- How did total e-commerce volume (₺) and number of transactions change from the pre-COVID period (2018–2019) to the post-COVID years (2022–2025)?
- Did the share of e-commerce within total retail trade remain permanently higher after the pandemic compared to before?
- Which sectors (such as electronics, fashion, and groceries) experienced the strongest and most persistent growth?
- How closely do online card spending trends correlate with overall e-commerce growth?

##  3. Data Sources
This project combines official open datasets, public ministerial announcements, and forecasting models to construct a complete view of Turkey’s e-commerce evolution from 2018 to 2025.
Due to the restructuring of the Ministry of Trade's ETBİS platform, some older PDF reports are no longer publicly accessible; therefore, verified announcements and sectoral publications are used for historical reconstruction.

🏛️ 1. Ministry of Trade — E-Commerce Announcements (2019–2023)

Official annual e-commerce volumes and transaction counts, obtained from ministerial press releases and verified public statements.

Provides:
- Annual e-commerce volume (₺)
- Annual number of transactions
- Overall trade share (%)
- Years covered: 2019, 2020, 2021, 2022, 2023

📘 2. TÜBİSAD / Deloitte Market Reports (2018)

Used to establish the pre-COVID baseline, including:
- 2018 market size
- Retail e-commerce ratio
- Early sector distribution

🏷️ 3. TÜİK — Retail Trade Volume Index

Offers baseline total retail activity necessary to compute:

- ecommerce_share = ecommerce_volume / total_retail_volume

💳 4. BKM — Card Spending Data

Includes:
Internet card spending
- Physical POS/in-store spending
- Total yearly card transactions
- Allows computation of:
- internet_card_share = internet_card_spending / total_card_spending

🔮 5. Forecasted Data (2024–2025)

Since no official data exists yet for 2024–2025, these years will be generated using a time-series forecasting model (Meta Prophet) trained on real 2018–2023 data.

Forecasts include:
- Predicted e-commerce volume (₺)
- Predicted number of transactions
- Confidence intervals

❗Forecasted values are labeled as estimated. The dataset will cover 2018–2025, with 2020–2021 defined as the pandemic intervention period dividing pre- and post-COVID phases.

##  4. Data Collection and Preparation Plan

 4.1 Collecting Historical Data (2018–2023)
In this step, I gather all reliable and publicly available data for Turkey’s e-commerce market from 2018 to 2023.

Data Sources Used:

- TÜBİSAD (2018 report) → Provides the pre-COVID baseline
- Ministry of Trade announcements (2019–2023) → Official yearly e-commerce volume and number of transactions
- TÜİK (Retail Trade Index) → Used to estimate the total retail market
- BKM (Card Payments Reports) → Internet vs. in-store card spending trends

❗All monetary values are converted to billion ₺ to keep the dataset uniform.


 4.2 Creating New Indicators

To better understand the data, I calculate several new metrics.

*Calculated Variables:*

    ecommerce_share = ecommerce_volume / total_retail_volume

    internet_card_share = internet_card_spending / total_card_spending

    growth_rate = pct_change(ecommerce_volume)


**Why these metrics matter**

    ecommerce_share → Shows how big e-commerce is inside the overall retail market

    internet_card_share → Shows if online payment behavior supports e-commerce growth

    growth_rate → Helps identify acceleration or slowdowns in the market


🔮 3. Forecasting 2024–2025

There is no official data yet for 2024 or 2025. So these years will be predicted using a time-series model. Forecasting is necessary to analyze long-term trends and to see if the COVID-19 growth effect continues beyond 2023.

*What the forecast provides:*

- Predicted e-commerce volume
- Predicted number of transactions
- Confidence intervals


⏳ 4. Splitting the Dataset into Time Periods

To answer the research questions clearly, the dataset is divided into three periods:

🟦 Pre-COVID (2018–2019) **Normal baseline period.**

🟨 COVID Impact (2020–2021) **Sharp changes caused by lockdowns and digital adoption.**

🟩 Post-COVID (2022–2025) **Stabilization and future trend (including forecast years).**


##  5. Analysis Plan
The analysis will compare pre-, during-, and post-COVID figures to detect structural differences in e-commerce behavior. Descriptive statistics will show changes in e-commerce share, transaction growth, and spending ratios. Correlation analysis will evaluate the relationship between internet card spending (from BKM) and total e-commerce volume (from the Ministry of Trade). If sectoral data are available, comparisons across industries will highlight which areas achieved the strongest and most sustained digital transformation. Results will be visualized through time-series charts, growth comparison plots, and percentage change visuals to make the shift clear and intuitive.

##  6. Expected Outcomes
This project is expected to show a significant structural increase in Turkey’s e-commerce market following the COVID-19 pandemic. Anticipated findings include:
- A sharp spike in 2020–2021 online transaction volumes.
- Continued high levels after 2022, proving the permanence of digital adoption.
- A strong positive correlation between online card payments and total e-commerce activity.
- Sector-specific differences showing that grocery and daily-consumption categories experienced the most rapid and lasting growth.

The results will offer quantitative evidence that COVID-19 accelerated Turkey’s transition toward a digitally driven retail economy and permanently transformed consumer shopping behavior.
