⚡ India Power Infrastructure Dashboard

An interactive Power BI dashboard analyzing India's power generation landscape — combining a self-curated dataset of 250+ power plants (capacity, fuel type, geolocation, ownership) with 8 years of state-wise electricity demand data to explore how India's generation capacity is distributed and how it compares against actual consumption.

🔗 Live Dashboard: [Add your Publish-to-Web link here]

📸 Screenshots below | 📁 Data  | 📊 Power BI file in root (.pbix)

🎯 Why I Built This

India's power sector is undergoing a major transition — coal-heavy legacy infrastructure alongside a fast-growing renewable push. I wanted to explore this shift with real, granular data rather than a pre-cleaned dataset, so I manually compiled plant-level information (including exact coordinates) to map and analyze the country's generation mix state by state, and combine it with public demand data to see how supply and consumption compare.

🗂️ Data Sources
Dataset	Description	Source
plants_data.csv	250+ power plants with capacity, fuel type, sector, owner, coordinates, commission year	Self-compiled from public records (CEA plant lists, company/state genco disclosures)


🛠️ Tools & Techniques
Power Query — unpivoted the wide-format demand data (29 state columns → long format) for proper data modeling
Data Modeling — star-schema style relationships joining plant and demand data on State
DAX — custom measures including Total Capacity, Renewable Share %, Capacity-to-Consumption Index, YoY growth
Geospatial Mapping — plant-level bubble map using latitude/longitude
Drillthrough & Bookmarks — state-level drillthrough page; collapsible filter panel via bookmark-toggle buttons

📊 Dashboard Pages

1. National Overview
KPI summary (total capacity, plant count, states covered, renewable share, average plant size), fuel-mix and sector-mix breakdowns, geospatial plant map, and state-wise capacity ranking.

2. Plant Explorer
Filterable plant-level view — slice by state, fuel type, sector, owner, status, and age group. Includes an owner-wise capacity breakdown and a searchable plant table.


🖼️ Screenshots

National Overview <img width="1357" height="768" alt="image" src="https://github.com/user-attachments/assets/b4bcd018-5cdc-4465-9226-adfa96f8535b" />

Plant Explorer <img width="1375" height="768" alt="image" src="https://github.com/user-attachments/assets/c949bf91-3682-48b9-9a66-d29ecb4c240c" />

🔍 Key Insights
India has nearly 242 power plants with a total capacity of around 248k MW in which ~18% is renewable share.
Coal-based plants account for ~71.41% of total installed capacity despite renewable capacity growing fastest post-2018
Gujarat has total 14 plants producing 20.88k MW capacity with Adani Mundra thermal power station producing highest power for the state.
The top 5 states hold roughly 75k MW of India's total installed capacity.
