# Cognifyz Restaurant Data Analysis

Python (Pandas, Matplotlib, Folium) analysis of a 9,551-restaurant, 21-column dataset provided during my Cognifyz Data Analyst internship (Jul-Aug 2026). The dataset is not included in this repo.

## Files
- `level1.ipynb`, `level2.ipynb`: the worksheet tasks as I submitted them (top cuisines, city analysis, price range, online delivery, ratings, cuisine combinations, geographic map, restaurant chains).
- `level1_cleaned.ipynb`, `level2_cleaned.ipynb`: my extension after the assignment, with data cleaning and re-checked results.

## Extension: data cleaning and reliability checks
- Filled 9 missing Cuisines values and confirmed 0 duplicate rows.
- Repaired 3 corrupted city names (Istanbul, Brasília, São Paulo). Remaining corrupted characters in the source file (restaurant names, addresses, localities, currency, cuisines) were flagged but not changed, since the original text can't be recovered.
- Found 2,148 restaurants (22%) with a rating of 0 (unrated) and excluded them from rating analysis, leaving 7,403 rated restaurants.
- Online delivery vs rating: the gap in the original analysis (3.25 vs 2.47) disappeared once unrated restaurants were excluded (3.38 with delivery vs 3.47 without), because unrated restaurants were concentrated among those without delivery.
- Top-rated cities (20+ rated restaurants): London 4.54, Orlando 4.48, Rest of Hawaii 4.41, Tampa Bay 4.41, Bangalore 4.38.
- Average votes per restaurant: 157 for all restaurants, 202 for rated ones.
- Most common rating range (rated only): 3.0 to 3.5 (34%).
- Top cuisines (20+ rated restaurants): Italian 3.95, American 3.92, Mexican 3.85.
- Top chains (5+ rated outlets): Chili's 4.58, Farzi Cafe 4.37, Barbeque Nation 4.35 (26 outlets), Punjab Grill 4.34.

## Other findings
- New Delhi holds 57% of listings; North Indian is the most common cuisine (9.8%).
- 46.5% of restaurants are in the lowest price tier.

## Tools
Python, Pandas, Matplotlib, Folium, Google Colab
