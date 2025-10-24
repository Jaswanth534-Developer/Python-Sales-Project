📂 Dataset Overview

Source: airbnb_data.csv
Description: Contains Airbnb listings information, including host details, neighbourhoods, prices, room types, number of reviews, and availability.

Key Columns:

name – Name of the listing

neighbourhood group – Main geographical area

neighbourhood – Specific location

room type – Type of accommodation

price – Price per night (USD)

minimum nights – Minimum number of nights required

number of reviews – Total reviews received

last review – Date of the latest review

availability 365 – Number of days available per year

service fee – Airbnb service fee

🧹 Step 1: Data Cleaning

Performed the following cleaning operations:

Price and fee conversion – Removed $ and , symbols and converted to numeric.

Date conversion – Converted last review to datetime format.

Type conversion – Converted key columns like minimum nights, number of reviews, and availability 365 to integers.

Missing values – Checked and handled missing values appropriately.

Dropped irrelevant columns – Removed unnecessary identifiers and duplicate metadata (e.g., id, host id, license).

📊 Step 2: Exploratory Data Analysis (EDA)
Key Analyses

Top 5 neighbourhood groups
Displayed the areas with the most Airbnb listings.

Room type distribution
Visualized the count of different room types using bar charts.

Price distribution
Examined overall price ranges and identified outliers.

Top 10 neighbourhoods by listings
Highlighted the most popular neighbourhoods.

Key Business Insights

Average Price by Room Type
Identified which room types are priced higher on average.

Most Expensive Neighbourhoods
Found top neighbourhoods with the highest average listing prices.

Listings with Most Reviews
Ranked listings by number of reviews to find popular hosts or properties.

🔍 Step 3: Correlation Analysis

Generated a correlation heatmap to explore relationships between numerical features such as:

price

minimum nights

number of reviews

availability 365

💾 Step 4: Save Cleaned Data

Saved the processed dataset for future use:

df.to_csv('cleaned_airbnb_data.csv', index=False)

🧠 Step 5: Insights & Recommendations
Key Findings

Entire home/apartment listings are typically the most expensive.

Certain neighbourhoods show consistently higher prices — possibly due to location demand.

The majority of listings have fewer reviews, suggesting many new or less popular hosts.

Recommendations

For hosts: Optimize pricing by comparing against similar listings in the same area.

For Airbnb: Promote listings in underrepresented neighbourhoods to balance supply and demand.

For travelers: Consider neighborhoods with lower prices but good review counts for better value.

🧰 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

📈 Future Work

Apply machine learning to predict listing prices.

Conduct sentiment analysis on review text.

Add geospatial visualization using Folium or Plotly.
