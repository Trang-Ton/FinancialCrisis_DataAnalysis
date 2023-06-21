# The Impact of Financial Crisis 2008 on European Firms’ Capital Structures

This report briefly shows the analysis results that represents European economy during the Financial Crisis times.

📈 Analyzed time period: 2004 - 2012

👭 Authors: Trang Ton and Quynh Phung

Raw data was extracted from [Osiris Database](https://www.bvdinfo.com/en-gb/our-products/data/international/osiris), which provides information on listed and unlisted firms worldwide, by Bureau van Dijk, a Moody's Analytics Company.

Python source code:

The study is intended to represent the EU economy, hence it includes companies from the Eurozone including 19 out of the 27 EU countries: 

🇦🇹 Austria, 🇧🇪 Belgium, 🇨🇾 Cyprus, 🇪🇪 Estonia, 🇫🇮 Finland, 🇫🇷 France, 🇩🇪 Germany, 🇬🇷 Greece, 🇮🇪 Ireland, 🇮🇹 Italy, 🇱🇻 Latvia, 🇱🇹 Lithuania, 🇱🇺 Luxembourg, 🇲🇹 Malta, 🇳🇱 Netherlands, 🇵🇹 Portugal, 🇸🇰 Slovakia, 🇸🇮 Slovenia, and 🇪🇸 Spain.

### 1. 🔎 Data filters:
✅ publicly traded and non-financial firms

✅ EU firms with using Euro currencies

✅ Accounting practice: IFRS - International Financial Reporting Standards

✅ Industry classification based on GICS codes

![](Industry.png)

### 2. Variables:
* Outcomes: leverage ratios
* Predictors: market capitalization, net sales, tangibility, return on assets ratios

![](Assets/DebtLeverageGraph.png)
*Figure 1 Debt leverage ratios over time 2004 - 2012*

The average debt leverage ratio clearly increased during the crisis years of 2008 and 2009. This implies that during the financial crisis, EU firms had higher debt compared to their assets.

![](Assets/CorrelationHeatmap.png)
*Figure 2: Correlation heatmap*

### 3. 🔑 Regression models:

Model (1), (2) table 1: OLS regression with time -fixed effect (Crisis period is taken as time based reference)

![](Assets/Table1.png)
*Table 1: OLS regression results*

Model (1), (3) table 2: Panel regression with time-fixed effects (Crisis period is taken as time based reference). Model (2), (4) table 2: Panel regression with interaction terms of 'ROA * Crisis period'& 'ROA * Post-crisis period'.

![](Assets/Table2.png)
*Table 2: Panel regression results*

### 4. 🚀 Implication of results:

💡 Both the OLS and panel regression results reveal the negative association between Leverage Ratio and Market Capitalisation and ROA but the positive relationship between Leverage Ratio and Firm Size. Tangibility appears insignificant to the changes of Leverage Ratio. 

💡 Most importantly, the financial crisis left huge financial damage on firms, pressuring firms to finance their business with internal funding and equity instead of loans and debts. The capital structure of firms in 19 European countries under study definitely changed post crisis.

#### 📖 References:
Caselli, S. and Negri, G. (2021) ‘Theoretical foundation of private equity and venture capital’, Private Equity and Venture Capital in Europe: Markets, Techniques and Deals (Third Edition), pp. 35-41

Rajan, G.R. and Zingales, L. (1995) ‘What do we know about Capital Structure? Some Evidence from International Data’, The Journal of France, Vol. L, No. 5, pp. 1421-1460









