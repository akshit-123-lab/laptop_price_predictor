# 💻 Laptop Price Predictor

This project explores and analyzes a dataset of laptops with the goal of understanding the factors that influence laptop pricing. It includes thorough data preprocessing, feature engineering, exploratory data analysis (EDA), and correlation analysis, all geared toward building an effective predictive model for laptop prices.

## 📊 Dataset

The dataset contains detailed information on over 1300 laptop models, including:
- Brand (Company)
- Product type and category
- Display specs (Screen size, resolution, IPS, Touchscreen)
- Processor details (Type, speed)
- RAM, storage (HDD, SSD, Flash)
- Graphics unit (GPU)
- Operating System
- Weight
- Price (converted to INR)

## 🔧 Features Engineered

- Extracted `X_res`, `Y_res`, `ppi` (pixels per inch) from screen resolution.
- Parsed `CPU` and `GPU` types into meaningful categories.
- Extracted individual storage types (HDD, SSD, Hybrid, Flash Storage).
- Cleaned and normalized OS, RAM, and weight data.
- Created binary flags for IPS panel and touchscreen features.
- Added numerical fields like CPU speed.

## 📈 Exploratory Data Analysis (EDA)

Performed detailed visual analysis using `seaborn`, `matplotlib`, and `plotly`, including:
- Price distribution across brands, types, screen sizes, and more.
- Price correlation with features like RAM, SSD, CPU speed, resolution, etc.
- Heatmaps and scatter plots for feature interactions and correlation understanding.

## 🔍 Key Insights

- RAM and SSD size have a strong positive correlation with price.
- High-resolution displays and IPS panels contribute to higher pricing.
- Laptops with dedicated GPUs like Nvidia GeForce or Quadro tend to be more expensive.
- Touchscreen and lightweight designs show moderate influence on pricing.
- Among processors, Intel Xeon and Ryzen Series are the priciest on average.

## 📦 Libraries Used

- `pandas`, `numpy` for data manipulation
- `matplotlib`, `seaborn`, `plotly` for visualization
- `scikit-learn` (optional for modeling in future work)

## 📌 Future Work

- Building machine learning models for accurate price prediction (Linear Regression, Random Forest, etc.)
- Feature importance analysis
- Web-based interface for live prediction input
