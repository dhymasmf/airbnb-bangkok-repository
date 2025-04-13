# Decoding What Drives Airbnb Success in Bangkok  
### A Multi-Factor Analysis of Listings, Location, and Behavior  

---

## Project Overview

This project is a capstone submission for Module 2 of the Data Science program at Purwadhika.  
We explore what drives **price** and **performance** of Airbnb listings in **Bangkok**, by analyzing factors such as location, reviews, room types, and host behavior.

Through this end-to-end data analytics pipeline, we prepare a polished dataset and deliver interactive **visual storytelling** using **Looker Studio**.

---

## 🔍 Problem Statement

> **What are the key factors that influence the success and pricing of Airbnb listings in Bangkok?**

We define success using:
- **Listing price**
- **Number of reviews**
- **Availability and demand**
- **Location/neighbourhood**
- **Host behavior (Superhost, listings count)**

---

## Tools & Technologies

| Tool | Purpose |
|------|--------|
| Python (pandas, numpy, seaborn, matplotlib) | Data cleaning & processing |
| Looker Studio | Dashboard & visualization |
| GitHub | Code versioning & hosting |
| VSCode | Main IDE |
| CSV | Raw dataset (Airbnb Listings Bangkok) |

---

## Dataset

The dataset was sourced from **Inside Airbnb** and contains information about:
- Listing ID, host ID
- Location (latitude, longitude, neighbourhood)
- Price
- Room type
- Number of reviews
- Availability
- Review metrics (per month, last 12 months)

 Files used:
- `airbnb_bangkok_cleaned.csv` — fully cleaned and processed dataset ready for visualization

---

## Data Cleaning & Processing

Steps taken:

1. **Removed duplicates** and irrelevant columns
2. **Handled missing values** (e.g., `reviews_per_month`)
3. **Converted data types** where needed
4. **Feature engineering**:
   - `is_superhost`: host type
   - `price_per_review`: value perception
   - `is_long_term`: derived from `minimum_nights`

5. **Correlation analysis** to assess numerical feature relevance
6. Final `df_model` was created by dropping:
   - `id`, `host_id`, `reviews_density`, `minimum_nights`

---

## Visualization in Looker Studio

 The final dashboard can be accessed here: [Click to View Dashboard](https://lookerstudio.google.com/reporting/1bedb78e-2d11-4759-9dda-e679e42dafd4)

### Visual Analysis Breakdown:

| Chart Type | Title | Insight |
|------------|-------|---------|
| Map | **Listings Density by Neighbourhood** | Visualizes listing concentration in key districts |
| Line Chart | **Price vs Number of Reviews** | Explore if higher prices affect reviews |
| Bar Chart | **Top Neighbourhoods by Listings** | Highlights areas with the most active listings |
| Pie Chart | **Distribution of Room Types** | Understand what room types are most popular |
| Filters | **Dynamic Exploration** | Slice data by `Room Type`, `Neighbourhood`, `Price` range |

---

## Key Insights

- **Location Matters**: Central areas like Sukhumvit dominate in listing counts and price.
- **Room Type Affects Price**: Entire homes significantly raise average pricing.
- **Superhosts Influence Perception**: Listings with Superhosts are more trusted and often better reviewed.
- **High Availability Correlates with Lower Price**: Possibly budget-friendly long-term stays.

---

## Conclusion

This project reveals the **multi-dimensional** nature of pricing and success on Airbnb.  
By cleaning, engineering, and visualizing the data, we now understand that **location**, **room type**, and **host behavior** collectively shape performance.

These insights are valuable for:
- **Hosts** who want to price and position listings better
- **Analysts** and **product teams** to design better marketplace experiences
- Future predictive modeling (Machine Learning)

---

## Links

- **Looker Studio Dashboard**: [View Here](https://lookerstudio.google.com/reporting/1bedb78e-2d11-4759-9dda-e679e42dafd4)
- **LinkedIn**: [Profile](https://www.linkedin.com/in/dhymasmf/)
- **Presentation**: [View Here](https://www.canva.com/design/DAGkXAU6TXU/8vJkI0g7L12PieqsE0xqEQ/edit?utm_content=DAGkXAU6TXU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

---

## Acknowledgements

Big thanks to:
- **Purwadhika**
- **Inside Airbnb** for open data
