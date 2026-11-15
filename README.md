# Why Does India Win Fewer Olympic Medals Than Its Population Suggests?
### A Data Analysis of Olympic Performance (1896-2024)

Data Analytics internship project by YOUR NAME

## Objectives
1. Analyze India's medal trends over time, by sport and by gender
2. Compare India with peer countries on medals per capita and per GDP
3. Identify India's strong, declining and growing sports
4. Test how much population, GDP and team size explain medal counts

## Data sources
All data is loaded by code. No data files are stored in this repository.
- Kaggle: *120 Years of Olympic History: athletes and results* (1896-2016)
- Kaggle: *Paris 2024 Olympic Summer Games*
- Kaggle: *2021 Olympics in Tokyo*
- World Bank API: population (SP.POP.TOTL) and GDP in current US$ (NY.GDP.MKTP.CD), 1960-2024

## Method
1. Kept Summer Games only and removed Art Competitions
2. Counted one medal per team per event, because team members appear as separate rows
3. Combined all Games (1896-2024) and matched Olympic and World Bank country codes
4. Validated India's medal totals against official results
5. Calculated medals per million people and per billion US$ of GDP, compared India with five peers (China, Brazil, Indonesia, Kenya, Japan), and fitted regression models

## Key findings
- India won 6 medals at Paris 2024, about one medal per 242 million people, and ranks last of six peers on medals per million people
- Hockey won 11 of India's 28 medals through 2016. Since 2000, medals have come from 5 sports, against 27 for China
- Population and GDP explain about 45% of the variation in medal counts (68% with team size). GDP is linked to medals, but population is not once GDP is included
- At Rio 2016 the model expected about 9.7 medals for India, and India won 2
- Among 80 countries with over 10 million people, India ranks 71st in over-performance

## Limitations
- Results show patterns, not causes
- Sport and gender data end at Rio 2016, because the Tokyo and Paris files contain country totals only
- GDP is in current US dollars, so medals per million people is the more reliable measure

## How to run
1. Open `Olympics_Analysis.ipynb` in Google Colab
2. Click **Runtime → Run all**

## Tools
Python, pandas, NumPy, Plotly, statsmodels, Google Colab
