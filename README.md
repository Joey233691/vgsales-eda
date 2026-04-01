# vgsales-eda
Exploratory data analysis on global video game sales (1980–2016) using Python
# 🎮 Video Game Sales — Exploratory Data Analysis
 
A data analysis project exploring global video game sales trends across platforms, genres, regions, and time periods using the VGChartz dataset.
 
---
 
## 📁 Project Structure
 
```
├── vgsales.csv                  # Raw dataset (16,598 records)
├── vgsales-eda.ipynb             # Main EDA notebook
├── vgsales-eda.html              # Exported HTML report
└── README.md
```
 
---
 
## 📊 Dataset Overview
 
| Attribute | Details |
|-----------|---------|
| Source | VGChartz |
| Records | 16,598 games |
| Columns | 11 (Rank, Name, Platform, Year, Genre, Publisher, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales) |
| Time Range | 1980 – 2016 |
 
---
 
## 🔍 Analysis Contents
 
### Data Cleaning
- Detected and removed 271 missing `Year` values and 58 missing `Publisher` values
- Stripped leading/trailing whitespace from categorical columns
- Converted `Year` dtype from `float` to `int`
- Confirmed no duplicate rows
 
### Exploratory Analysis
- **Categorical variables**: 31 platforms, 12 genres, 576 publishers
- **Numerical summary**: Global sales are right-skewed (mean 0.54M, max 82.74M), reflecting a long-tail distribution
- **Regional correlation**: NA and EU sales are the strongest predictors of global sales
 
### Visualisations
 
| # | Chart | Key Finding |
|---|-------|-------------|
| 1 | Line chart — Global Sales by Year | Sales peaked around 2008–2010 then declined |
| 2 | Bar chart — Sales by Genre | Action is the top-selling genre, followed by Sports and Shooter |
| 3 | Heatmap — Regional Sales Correlation | NA sales most strongly correlated with global sales |
| 4 | Scatter plot — Individual Game Sales | Long-tail effect: a few blockbuster titles dominate total sales |
| 5 | Grouped bar chart — Regional Sales by Platform | X360, Wii, PS2 dominate NA; regional preferences vary significantly |
 
---
 
## 💡 Key Findings
 
1. **Action games dominate**: Action is the best-selling genre globally, with Sports and Shooter genres also performing strongly.
2. **Peak era: 2008–2010**: Global game sales surged from 1995, peaked around 2008–2010, then declined — likely reflecting the rise of mobile gaming.
3. **North America leads**: NA sales are most highly correlated with global performance, making it the most influential regional market.
4. **Blockbuster effect**: A small number of games (e.g. Wii Sports at 82.74M) account for a disproportionate share of total sales.
5. **Platform-region preferences**: Japanese and other-region markets show distinct platform preferences compared to NA and EU.
 
---
 
## 🛠 Dependencies
 
```
pandas
numpy
matplotlib
seaborn
scipy
```
 

 
---
 
## 👤 Author
 
**Ying Qiao · MSc Information Systems, University College Dublin
joey2330000@gmail.com · LinkedIn · GitHub** 
 
