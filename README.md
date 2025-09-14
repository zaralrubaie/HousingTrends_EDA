# HousingTrends_EDA
# Property_EDA_Visualizations

## Overview
This project performs a comprehensive **Exploratory Data Analysis (EDA)** on a real estate dataset.  
It focuses on uncovering patterns, trends, and insights from property listings to better understand the housing market.

The dataset includes **train and test sets** with features such as property type, size, status, and price.  
The analysis highlights **data visualization skills** using Python, Matplotlib, and Seaborn, along with clear Markdown explanations.

---

## Dataset Features

| Feature | Description |
|---------|-------------|
| POSTED_BY | Who listed the property (Dealer, Owner, Builder) |
| UNDER_CONSTRUCTION | Whether the property is under construction |
| RERA | Whether the property is RERA registered |
| BHK_NO. | Number of bedrooms |
| BHK_OR_RK | BHK or RK property type |
| SQUARE_FT | Area of the property in sq. ft |
| READY_TO_MOVE | If the property is ready to move |
| RESALE | Resale or new property |
| ADDRESS | Property address |
| LONGITUDE | Longitude coordinate |
| LATITUDE | Latitude coordinate |
| TARGET(PRICE_IN_LACS) | Property price in lacs (target variable) |

---

## Exploratory Data Analysis (EDA)

### 1. Categorical Feature Distributions

**POSTED_BY Distribution**  
![POSTED_BY](plots/01_posted_by_distribution.png)  
> Most properties are listed by **Dealers**, followed by **Owners** and **Builders**, indicating dealer-dominated listings.

**UNDER_CONSTRUCTION**  
![UNDER_CONSTRUCTION](plots/02_under_construction.png)  
> Majority of properties are **not under construction**, showing a market preference for completed properties.

**READY_TO_MOVE**  
![READY_TO_MOVE](plots/03_ready_to_move_pie.png)  
> Around **82% of properties are ready to move**, highlighting availability for immediate possession.

**RESALE**  
![RESALE](plots/04_resale_distribution.png)  
> Most properties are **resale**, suggesting previously owned properties dominate the market.

**BHK_OR_RK**  
![BHK_OR_RK](plots/05_bhk_or_rk_distribution.png)  
> Majority of properties are **BHK units**, indicating standard multi-room apartments dominate the market.

---

### 2. Numerical Feature Distributions

**Square Feet Distribution**  
![SQUARE_FT](plots/06_square_ft_distribution.png)  
> Most properties have smaller areas (~35,000 sq.ft), but a few large properties exist (up to 250,000 sq.ft), creating a right-skewed distribution.

**Price Distribution (TARGET)**  
![PRICE](plots/07_target_price_distribution.png)  
> Property prices are mostly on the lower end with a few high-value outliers, showing a right-skewed distribution.

---

### 3. Train vs Test Comparison

**POSTED_BY: Train vs Test**  
![POSTED_BY Train vs Test](plots/08_posted_by_train_vs_test.png)  
> Both datasets show similar distributions, with **Dealers** listing most properties, followed by **Owners** and **Builders**.

**SQUARE_FT: Train vs Test**  
![SQUARE_FT Train vs Test](plots/09_square_ft_train_vs_test.png)  
> The distributions are similar, but the test set has a slightly higher peak density (~2) compared to train (~1.23), indicating clustering of property sizes.

---

### 4. Insights & Summary
- Dealers dominate property listings in both train and test datasets.  
- Most properties are ready-to-move and resale, highlighting buyer preference for completed properties.  
- The market is dominated by BHK units and smaller properties, but high-value and large-area properties exist as outliers.  
- Train and test sets are consistent in feature distributions, making them reliable for further analysis.  

---

## Technologies Used
- Python 3  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Jupyter Notebook / Google Colab  

---

## Project Structure

