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

## 1. Categorical Feature Distributions

The project includes visualizations for key categorical features:  

- **POSTED_BY** – Distribution of property listings by Dealers, Owners, and Builders.  
- **UNDER_CONSTRUCTION** – Shows the count of properties under construction vs. completed.  
- **READY_TO_MOVE** – Percentage of properties ready to move vs. not.  
- **RESALE** – Count of resale vs. new properties.  
- **BHK_OR_RK** – Comparison of BHK vs. RK properties.  

> All comparison plots are saved in the `EDA - PLOTS.zip` file. Full analysis and insights are available in the `EDA-data.py` script.

---

## 2. Numerical Feature Distributions

The project includes visualizations for key numerical features:  

- **Square Feet Distribution** – Shows the distribution of property sizes. Most properties have smaller areas (~35,000 sq.ft), but a few large properties exist (up to 250,000 sq.ft), creating a right-skewed distribution.  
- **Price Distribution (TARGET)** – Shows the distribution of property prices. Most properties are priced on the lower end, with a few high-value outliers, creating a right-skewed distribution.  

> All comparison plots are saved in the `EDA - PLOTS.zip` file. Full analysis and insights are available in the `EDA-data.py` script.

---

## 3. Train vs Test Comparison

The project also includes visual comparisons between train and test datasets for key features:  

- **POSTED_BY: Train vs Test** – Both datasets show similar distributions, with **Dealers** listing most properties, followed by **Owners** and **Builders**.  
- **SQUARE_FT: Train vs Test** – The distributions are similar, but the test set has a slightly higher peak density (~2) compared to the train set (~1.23), indicating clustering of property sizes.  

> All comparison plots are saved in the `EDA - PLOTS.zip` file. Full analysis and insights are available in the `EDA-data.py` script.

---

## 4. Insights & Summary
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
````
Property_EDA_Visualizations/
│
├── EDA - PLOTS.zip        # Contains all saved plot images
├── EDA-data.py            # Python script with EDA code and explanations
├── LICENSE                # MIT License file
└── README.md              # Project overview, explanations, and instructions
> To view all the plots, download and extract the `EDA - PLOTS.zip` file.
````
## Notes
- All plots are inside the zip file. You can extract it to view the images.
- Detailed explanations for each visualization are included in EDA-data.py.
## ## License
This project is licensed under the [MIT License](LICENSE).
