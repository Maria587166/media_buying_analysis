# media_buying_analysis
Comparing ad platform efficiency (ROAS/CPA) across Google, Meta, and TikTok using Excel and Tableu
Overview 

Comparison of advertising performance across Google, Meta, and TikTok to determine 

which platform delivers the best return on ad spend, and where budget should 

realistically reallocated. 

Business Question 

Which advertising platform delivers the best efficiency (ROAS/CPA), and how should 

that shape budget allocation across channels? 

Dataset 

Real public dataset from Kaggle, Global Ads Performance (Google, Meta, TikTok) — 

1,800 campaign rows from 2024, with spend, impressions, clicks, conversions, revenue, 

ROAS, CPA, campaign type, industry, and country. 

Kaggle dataset - https://www.kaggle.com/datasets/nudratabbas/global-ads-performance-google-meta-tiktok/data  

Tools & Methodology 

1. Excel 

Pivot table: spend and revenue by platform 

ROAS (revenue/spend) and CPA (spend/conversions) were recalculated manually 

with formulas rather than relying on the pre-built columns in the dataset, to verify 

and demonstrate the underlying logic 

Three t-tests (Data Analysis ToolPak): pairwise comparison of CPA between 

platforms 

Correlation (CORREL) between ad spend and ROAS at the individual campaign level 

2. Tableau - Interactive Dashboard, ROAS by platform (bar chart) 

Monthly ROAS trend split by platform (line chart) 

Ad Spend vs ROAS scatter plot with a trend line  

Filters for platform and month applied across all views 

Key Findings 

1. TikTok is the most efficient platform on both metrics at once 

Platform       Spend Revenue  ROAS               CPA 

Google Ads  $6,349,269         $22,033,745     3.47x $48.43 

Meta Ads      $2,106,062         $11,926,046    5.66x $28.75 

TikTok Ads  $2,653,419         $20,223,540     7.62x $21.67 

2. All CPA differences between platforms are statistically significant Three t-tests 

(Google vs. TikTok, Google vs. Meta, Meta vs. TikTok) all showed statistically significant 

differences (p < 0.001), indicating a stable efficiency ranking rather than random 

variation. 

3. Google receives almost 60% of the total budget despite being the weakest 

performer Despite getting the largest share of spend ($6.3M of $11.1M total budget), 

Google has the lowest ROAS and the highest CPA of the three platforms. 

4. The platform ranking is stable all year The monthly ROAS trend shows that TikTok > Meta > Google holds throughout all of 2024, with no crossover at any point, 

confirming the difference is structural rather than seasonal. 

5. Campaign budget size is only weakly related to efficiency The correlation 

between ad spend and ROAS at the individual campaign level is weak and negative (r = 

-0.255, R^2 = 0.065, p < 0.001), confirmed independently in both Excel and Tableau. The 

relationship is statistically significant but explains only about 6.5% of the variation in 

ROAS - platform choice matters more than the size of an individual campaign’s budget. 

Limitations 

Because the spend-to-ROAS correlation is weak, this analysis can’t confidently claim a strong “diminishing returns” effect from spend alone; other factors like platform, 

campaign type, and industry likely matter more. 

Repository Contents 

File  

Description 
global_ads_performance_dataset.xlsx - Pivot table, ROAS/CPA calculations, t-tests, 

dashboard_preview.png - correlation Screenshot of the final Tableau dashboard 

 

live Tableau Public dashboard https://public.tableau.com/app/profile/maria.medvedieva2019/viz/Book1_17702902469590/Dashboard1?publish=yes  

How to Explore 

1. Excel: open global_ads_performance_dataset.xlsx, review the pivot table and the t- 

test/correlation sheets 

2. Tableau: view the https://public.tableau.com/app/profile/maria.medvedieva2019/viz/Book1_17702902469590/Dashboard1?publish=yes live dashboard in Tableau 

Author 

Maria M. - Business Analytics student
