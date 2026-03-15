# 🏙️ Dubai Real Estate Analytics Dashboard (Power BI)

## 📌 Project Overview
This interactive Power BI dashboard analyzes 50,000 property listings across the Dubai real estate market. It leverages DAX to engineer custom data features—including pricing tiers, property types, and developer market share—while featuring dynamic KPI tracking, geospatial mapping, and interactive slicers for deep-dive market exploration. Ultimately, the project delivers actionable, data-driven insights to help real estate investors and agents identify high-value opportunities.

![Dashboard Preview](Insert_Your_Screenshot_Link_Here)

## 🎯 Business Objectives
* Analyze the average cost of real estate across key Dubai neighborhoods (Downtown, Arabian Ranches, Al Qudra).
* Evaluate how property age, square footage, and bedroom count impact the final listing price.
* Identify which developers and property types hold the largest market share.

## 🛠️ Tech Stack & Skills
* **Tool:** Microsoft Power BI
* **Languages:** DAX (Data Analysis Expressions)
* **Skills:** Data Modeling, Geospatial Analytics, Advanced Visualizations, Business Intelligence

## 🧮 Data Engineering & DAX Logic (Back-End)
The raw dataset was enriched using advanced DAX calculations to simulate a realistic, localized Dubai market:
* **`PricePerSqft`**: Established a baseline valuation metric (`Price / SquareFeet`).
* **`ListingCategory`**: Segmented the market into Budget, Mid-Range, and High-End tiers using the `PERCENTILE.INC` function.
* **`Dubai Location`**: Mapped generic zones to specific, highly recognizable communities (e.g., Downtown Dubai, Arabian Ranches) for geospatial mapping.
* **`Developer Market Share`**: Distributed properties dynamically among top developers (Emaar, DAMAC, Sobha, Nakheel) using a Modulo mathematical function `MOD(SquareFeet, 4)`.
* **`Property Type & Furnishing`**: Simulated using `SWITCH` statements based on bedroom and bathroom counts.

## 📊 Visual Analytics (Front-End)
The dashboard provides a highly interactive user experience through the following visuals:
* **Geospatial Map:** Plots average property values across specific Dubai coordinates.
* **Min/Avg/Max Column Chart:** Displays the exact price distribution and spread by neighborhood.
* **Scatter Plot:** Illustrates the correlation between property size, price, and listing tier.
* **Dynamic KPIs:** Tracks total listings, average price, and oldest property age.
* **Interactive Slicers:** Allows users to drill down by Bedrooms, Bathrooms, Neighborhood, Tier, and Price Range.

## 💡 Key Insights & Recommendations
1. **Value Drivers:** The highest-priced "High-End" properties are driven more by total square footage than strictly by the number of bedrooms.
2. **Investor Action:** Target *Mid-Range* properties in suburban areas (e.g., Arabian Ranches) to achieve the best balance of square footage and entry price for long-term appreciation.
3. **Agent Action:** Focus primary marketing and lead-generation efforts on 3-to-4-bedroom homes (Townhouses and Villas), as they represent a highly liquid, in-demand segment of the market.

## 🚀 How to Use
1. Clone this repository to your local machine.
2. Open the `Dubai_Real_Estate_Dashboard.pbix` file in Power BI Desktop.
3. Interact with the slicers on the left panel to dynamically filter the data by location, price range, and property type.
