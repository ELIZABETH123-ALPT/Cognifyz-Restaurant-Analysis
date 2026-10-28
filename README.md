# Cognifyz Restaurant Analysis

Python (Pandas, Matplotlib, Folium) analysis of a 9,551-restaurant, 21-column dataset provided during my Cognifyz Data Analyst internship (Jul-Aug 2026). The dataset is not included in this repo.

## Files

* `level1.ipynb`, `level2.ipynb`: the worksheet tasks as I submitted them (top cuisines, city analysis, price range, online delivery, ratings, cuisine combinations, geographic map, restaurant chains).
* `level1_cleaned.ipynb`, `level2_cleaned.ipynb`: my extension after the assignment, with data cleaning and re-checked results.

## Data Cleaning

* Filled 9 missing Cuisines values with "Unknown" and confirmed 0 duplicate rows.
* Repaired 3 corrupted city names (Istanbul, Brasília, São Paulo). Remaining corrupted characters in the source file (restaurant names, addresses, localities, currency, cuisines) were flagged but not changed, since the original text can't be recovered.
* Found 2,148 restaurants (22%) with a rating of 0 (unrated) and excluded them from rating analysis, leaving 7,403 rated restaurants.

## Key Findings

* **Online delivery vs rating:** In the original analysis, restaurants with online delivery averaged 3.25 and those without averaged 2.47. After excluding unrated restaurants, the averages were 3.38 with delivery and 3.47 without, so the gap reversed slightly. Unrated restaurants were concentrated among those without delivery, which had been pulling their average down.
* **Online delivery availability:** Only about 26% of restaurants offer online delivery.
* **Top-rated cities** (20+ rated restaurants): London 4.54, Orlando 4.48, Rest of Hawaii 4.41, Tampa Bay 4.41, Bangalore 4.38.
* **Top cuisines** (20+ rated restaurants): Italian 3.95, American 3.92, Mexican 3.85.
* **Top chains** (5+ rated outlets): Chili's 4.58, Farzi Cafe 4.37, Barbeque Nation 4.35 (26 outlets), Punjab Grill 4.34.
* **Votes:** Average votes per restaurant: 157 for all restaurants, 202 for rated ones.
* **Ratings:** The most common rating range (rated only) is 3.0 to 3.5 (34%).
* **Listings:** New Delhi holds 57% of listings; North Indian is the most common cuisine (9.8%).
* **Pricing:** 46.5% of restaurants are in the lowest price tier.

## Tools

Python, Pandas, Matplotlib, Folium, Google Colab
