# 🇹🇷 COVID-19 and the Rise of E-Commerce in Turkey (2018–2025)

## 🛒 Introduction
This project explores how Turkey’s e-commerce market evolved before, during, and after the COVID-19 pandemic. The pandemic created one of the most rapid transitions to online shopping in modern history as lockdowns and restrictions forced consumers and businesses to shift to digital platforms. By analyzing official national datasets from 2018 to 2025, this project aims to understand whether the surge in e-commerce during COVID-19 was a short-term effect or a lasting structural change in Turkey’s retail landscape.

## 🎯 1. Motivation
COVID-19 dramatically reshaped global consumer behavior. In Turkey, the e-commerce sector grew at record speed as households adopted digital shopping out of necessity. As restrictions were lifted, an important question emerged:

> Has the shift toward online retail remained permanent, or did consumer habits revert to traditional physical shopping?

Understanding this transformation is crucial for analyzing Turkey’s economic digitalization, business strategies, and long-term consumer adaptation. This project seeks to provide a data-driven overview of how the pandemic accelerated digital transformation and changed the retail structure of Turkey’s economy.

## ❓ 2. Research Questions
- How did total e-commerce volume (₺) and number of transactions change from the pre-COVID period (2018–2019) to the post-COVID years (2022–2025)?
- Did the share of e-commerce within total retail trade remain permanently higher after the pandemic compared to before?
- Which sectors (such as electronics, fashion, and groceries) experienced the strongest and most persistent growth?
- How closely do online card spending trends correlate with overall e-commerce growth?

## 📊 3. Data Sources
- **E-Ticaret Bilgi Platformu – Ministry of Trade:** Official e-commerce statistics including annual transaction volumes, growth rates, and total retail share.  
  🔗 https://www.eticaret.gov.tr/istatistikler  
- **BKM – Bankalararası Kart Merkezi:** Card transaction data (internet vs. in-store spending), representing consumer payment trends.  
  🔗 https://bkm.com.tr/raporlar-ve-yayinlar/donemsel-bilgiler/  
- **TÜİK – Turkish Statistical Institute:** Retail trade and services indices providing baseline total retail activity.  
  🔗 https://data.tuik.gov.tr/Kategori/GetKategori?p=ticaret-ve-hizmet-115  

The dataset will cover 2018–2025, with 2020–2021 defined as the pandemic intervention period dividing pre- and post-COVID phases.

## 🧠 4. Data Collection and Preparation Plan
Data will be collected from the Ministry of Trade, BKM, and TÜİK official portals. E-commerce volumes will be merged with card transaction data to create yearly comparisons of online vs. physical spending. All monetary values will be standardized into billion ₺ units, and derived indicators such as:
- `ecommerce_share = ecommerce_volume / total_retail_volume`
- `internet_card_share = internet_card_spending / total_card_spending`
will be calculated. The dataset will then be divided into three time frames: Pre-COVID (2018–2019), COVID period (2020–2021), and Post-COVID (2022–2025). Visualization will include line and bar plots highlighting the pandemic period and trend differences.

## 📈 5. Analysis Plan
The analysis will compare pre-, during-, and post-COVID figures to detect structural differences in e-commerce behavior. Descriptive statistics will show changes in e-commerce share, transaction growth, and spending ratios. Correlation analysis will evaluate the relationship between internet card spending (from BKM) and total e-commerce volume (from the Ministry of Trade). If sectoral data are available, comparisons across industries will highlight which areas achieved the strongest and most sustained digital transformation. Results will be visualized through time-series charts, growth comparison plots, and percentage change visuals to make the shift clear and intuitive.

## 🧩 6. Expected Outcomes
This project is expected to show a significant structural increase in Turkey’s e-commerce market following the COVID-19 pandemic. Anticipated findings include:
- A sharp spike in 2020–2021 online transaction volumes.
- Continued high levels after 2022, proving the permanence of digital adoption.
- A strong positive correlation between online card payments and total e-commerce activity.
- Sector-specific differences showing that grocery and daily-consumption categories experienced the most rapid and lasting growth.

The results will offer quantitative evidence that COVID-19 accelerated Turkey’s transition toward a digitally driven retail economy and permanently transformed consumer shopping behavior.
