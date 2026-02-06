# poland-real-estate-price-analysis
Exploratory analysis of 15,521 apartments across 15 Polish cities. Identified key price factors: square meters (0.64 correlation), rooms (0.51), and property condition (+33% premium vs low). Handled 76% missing data strategically. Built with Python, pandas, matplotlib. Demonstrates data cleaning, statistical analysis, and visualization skills.

# Poland Real Estate Price Analysis

Exploratory Data Analysis (EDA) of apartment prices across 15 major Polish cities to identify key factors influencing property valuations.

## 📊 Project Overview

This project analyzes **15,521 apartment listings** from Poland's largest cities to answer key questions:
- What factors drive apartment prices?
- How does property condition affect valuation?
- What's the price difference between cities?
- Do amenities like parking and balconies impact price?

## 🎯 Business Problem

Real estate agencies and property buyers need to understand:
- Which features add the most value to apartments
- How to accurately estimate property prices
- Market trends across different Polish cities

## 📁 Dataset

- **Source:** Polish real estate listings
- **Size:** 15,521 apartments
- **Features:** 28 columns including:
  - Price, location (city, coordinates)
  - Physical characteristics (area, rooms, floor)
  - Building info (year built, material, condition)
  - Amenities (parking, balcony, elevator, security)
  - Infrastructure (distances to schools, clinics, restaurants)
- **Cities:** Warsaw, Krakow, Wroclaw, Gdansk, Lodz, and 10 others

## 🔍 Key Findings

### 1. **Top Price Factors**
- **Square meters:** 0.64 correlation (strongest factor)
- **Number of rooms:** 0.51 correlation
- **Infrastructure (POI count):** 0.20 correlation

### 2. **Property Condition Impact**
- Premium apartments: 877k PLN average
- Low condition apartments: 658k PLN average
- **Difference:** +33% for premium vs low condition
- **Insight:** 76% of listings don't specify condition - these properties have similar prices to premium (823k PLN)

### 3. **Building Age vs Condition**
- Premium properties: median built in 2009
- Unknown condition: median built in 2000
- Low condition: median built in 1970
- **Insight:** Age and condition are separate factors - old apartments in prime locations can cost more than new ones in suburbs

### 4. **Missing Data Patterns**
- 76% missing `condition` data
- 39% missing `buildingMaterial` data
- **Solution:** Created "unknown" category instead of dropping - these properties show distinct price patterns

