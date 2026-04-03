# Experiment 14: Data Binning and Data Formatting Using Python

**Name:** Arhan Nair  
**PRN:** 25070123169  


---

## 1. Theory

### Data Binning
**Data binning** (or bucketing) is a data preprocessing technique used to group a set of continuous values into a smaller number of "bins" or categories. This helps in reducing the impact of minor observation errors and makes numerical data easier to analyze for categorical patterns. In Pandas, this is typically achieved using the `pd.cut()` function.


### Data Formatting
**Data formatting** involves standardizing the format of data so that it is consistent across the entire dataset. This includes:
* **Type Conversion**: Changing data types (e.g., converting an `int` to a `float`) using `.astype()`.
* **String Standardization**: Converting text to a uniform case (uppercase or lowercase) using `.str.upper()` or `.str.lower()`.
* **Rounding**: Limiting the number of decimal places for numerical precision using `.round()`.

---

## 2. Implementation Overview

### Product Sales Dataset
The experiment first utilized a product dataset containing **Product**, **Price**, and **Units_Sold**.
* **Price Binning**: Prices were categorized into "LOW", "MEDIUM", and "HIGH" based on specific ranges (0-10k, 10k-30k, 30k-60k).
* **Formatting**: The "Product" names were standardized to uppercase (e.g., `LAPTOP`), and "Units_Sold" was converted to a `float` data type for more precise calculations.

### Order Value Dataset
A second dataset focused on **Order_ID** and **Order_Value** was used to demonstrate more granular binning.
* **Categorization**: Order values were sorted into five bins: "Low", "Medium", "High", "Very High", and "Extremely High".
* **Statistical Summary**: Using `value_counts()`, it was determined that the "Medium" and "High" categories each contained 3 orders, while "Low" had 2.

---

## 3. Conclusion

This experiment demonstrates how preprocessing techniques like binning and formatting transform raw numbers into meaningful business segments. Standardizing data ensures that analysis is accurate and that categories are easily interpretable for decision-making.


**Key Takeaways:**
* **Categorical Conversion**: Binning allows for a transition from numerical analysis to categorical analysis, which is useful for identifying "High Value" vs "Low Value" segments.
* **Data Consistency**: Formatting operations like `.str.upper()` prevent duplicate entries caused by casing differences and ensure clean data visualization.
* **Operational Precision**: Converting data types and rounding values ensures that numerical operations remain consistent across different platforms or libraries.

---
