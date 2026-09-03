# 💎 Statistical Diamond Prices

A Python data visualization project that explores the **distribution of diamond prices across different diamond cut qualities** using the Seaborn `diamonds` dataset.

The project uses a **boxen plot** to visualize the distribution and statistical characteristics of diamond prices for each cut category.

## 📌 Project Overview

The goal of this project is to understand how **diamond cut quality relates to price distribution**.

A sample of 1,000 diamonds is selected from the Seaborn dataset, and their prices are compared across different cut categories.

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Seaborn**
* **Matplotlib**

## 📊 Visualization

The project creates a **Boxen Plot** (also known as a letter-value plot).

A boxen plot is useful for visualizing the distribution of large datasets and provides more information about the tails of the distribution than a traditional box plot.

The visualization compares:

* **X-axis:** Diamond cut quality
* **Y-axis:** Diamond price
* **Sample size:** 1,000 diamonds

## 💻 Code

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Load and sample the diamonds dataset
data = sns.load_dataset("diamonds").sample(1000)

# Create boxen plot
sns.boxenplot(
    data=data,
    x="cut",
    y="price"
)

# Customize the chart
plt.title("Diamond Price Distribution")
plt.xticks(rotation=20)

# Display the visualization
plt.show()
```

## 🔍 Statistical Analysis

The boxen plot helps identify:

### 1. Price Distribution

Shows how diamond prices are distributed within each cut category.

### 2. Median and Central Tendency

The visualization provides insight into where the central portion of prices lies for each cut.

### 3. Spread

The vertical spread indicates how widely diamond prices vary within each cut category.

### 4. Outliers and Extreme Values

The plot helps reveal diamonds with unusually high or low prices relative to other diamonds in their cut category.

### 5. Comparison Between Cuts

Different cut qualities can be compared to understand differences in their price distributions.

## 📈 Dataset

The dataset is the built-in **diamonds dataset** provided by Seaborn.

It contains information about approximately 54,000 diamonds, including variables such as:

* `carat` — Diamond weight
* `cut` — Quality of the cut
* `color` — Diamond color
* `clarity` — Diamond clarity
* `depth` — Total depth percentage
* `table` — Width of the top relative to length
* `price` — Diamond price
* `x` — Length
* `y` — Width
* `z` — Depth

This project uses the `cut` and `price` columns.

## 🎯 Learning Objectives

This project demonstrates how to:

* Load built-in datasets using Seaborn
* Randomly sample observations from a dataset
* Create statistical visualizations
* Use boxen plots for distribution analysis
* Compare numerical variables across categorical groups
* Customize Matplotlib charts
* Communicate statistical insights visually

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/statistical-diamond-prices.git
```

### 2. Navigate into the project

```bash
cd statistical-diamond-prices
```

### 3. Install dependencies

```bash
pip install pandas seaborn matplotlib
```

### 4. Run the Python script

```bash
python diamond_prices.py
```

## 📁 Project Structure

```text
statistical-diamond-prices/
│
├── diamond_prices.py
├── README.md
└── requirements.txt
```

## 📌 Key Takeaway

This project demonstrates how statistical visualization can be used to investigate **diamond price distributions across different cut qualities**. The boxen plot provides a detailed view of the spread and shape of the price data.

---

⭐ **If you found this project useful, consider giving the repository a star!**
