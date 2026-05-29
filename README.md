# Zomato Restaurant Data Analysis

This project is all about exploring and understanding the Zomato restaurant dataset for Bangalore. We do a full Exploratory Data Analysis (EDA) using Python to find useful patterns and insights about restaurants, their ratings, cuisine types, locations, and pricing.

---

## What This Project Does

We load the raw Zomato dataset, clean it up, and then create visualizations to answer questions like:

- Which areas in Bangalore have the most restaurants?
- What are the most popular cuisines?
- Does a higher price actually mean a better rating?
- How are ratings, votes, and cost related to each other?

---

## Dataset

The dataset used is `zomato.csv` which contains info about restaurants listed on Zomato in Bangalore. It includes details like location, cuisines, ratings, cost for two people, restaurant type, and whether online ordering is available.

---

## Libraries Used

| Library | Purpose |
|---|---|
| pandas | Data loading and manipulation |
| numpy | Numerical operations |
| matplotlib | Plotting graphs |
| seaborn | Better looking statistical plots |
| wordcloud | Generating word cloud from cuisine names |

---

## Steps Followed

**1. Data Loading**
Load the CSV file and check its shape and columns.

**2. Data Cleaning**
- Dropped unnecessary columns like url, address, phone, dish liked, menu item
- Renamed columns for easier access (like cost_for_two and area)
- Cleaned the rating column by removing the /5 suffix and handling invalid values like NEW or -
- Cleaned the cost column by removing commas
- Dropped rows with missing rating or cost values
- Filled missing cuisine and restaurant type with default values

**3. Basic Statistics**
Printed key numbers like total restaurants analyzed, average rating, average cost for two, and the most expensive restaurant.

**4. Visualizations**

- Bar chart of Top 10 Restaurant Hotspots in Bangalore
- Horizontal bar chart of Top 15 Most Popular Cuisines
- Scatter plot comparing Cost vs Rating (also colored by online order availability)
- Heatmap showing correlation between Rating, Votes, and Cost
- WordCloud of all cuisine names

---

## How to Run This

1. Make sure you have Python installed (3.7 or above is fine)

2. Install the required libraries by running this in your terminal:

```bash
pip install pandas numpy matplotlib seaborn wordcloud
```

3. Place the `zomato.csv` file in the same folder as the notebook

4. Open the notebook in Jupyter and run all cells from top to bottom

```bash
jupyter notebook Task_1.ipynb
```

---

## Key Insights

- Some areas in Bangalore are way more packed with restaurants than others
- North Indian and Chinese are among the most common cuisines
- Price does not always guarantee a better rating
- Votes and ratings tend to have some correlation but cost does not strongly affect rating

---

## File Structure

```
project/
│
├── Task_1.ipynb      # Main notebook with all analysis
├── zomato.csv        # Dataset (download separately)
└── README.md         # This file
```

---

## Author

Engineering Student Project | Exploratory Data Analysis Task
