# Skin-Care-Product-Web-Scraping

# 🧴 Cosmetic Product Similarity Analysis Based on Ingredients

This project analyzes the similarity of cosmetic products based on their ingredient lists. The main goal is to identify products that share one or more ingredients and to uncover clusters of items with overlapping formulations.

---

## ✅ Key Steps:

### 1. Web Scraping:
- Used `requests` and `BeautifulSoup` to extract product names, URLs, and ingredient lists from a static cosmetic store website.
- Since the site had no unique identifiers for ingredients, a known ingredient list was used to locate relevant data in each HTML page.

### 2. Data Processing:
- Cleaned and standardized ingredients into structured lists.
- Compared each product’s ingredients with all others to:
  - Find products with at least one shared ingredient.
  - Count the number of matching products.
  - Count the number of unique shared ingredients.

### 3. Visualization:
- Created an interactive scatter plot with `plotly.express`:
  - **X-axis:** Number of unique shared ingredients.
  - **Y-axis:** Number of matching products.
  - **Hover:** Displays product title and shared ingredients.
  - **Bubble size and color:** Reflect number of matches.
- Insight: Frequently used ingredients and product similarities became visually evident.

### 4. Grouping Products:
- Grouped products with identical sets of shared ingredients.
- Assigned group labels (A, B, C...) and presented a clear summary table.

---

## 🎯 Inference:
- Revealed ingredient-based relationships across products.
- Identified clusters of similar formulations, useful for:
  - Product recommendation engines
  - Competitive market analysis
  - Optimizing new product formulations

All Python code is available in the notebook for full reproducibility.
