# Maji-Ndogo-water-access-and Infrastructure-dashboard
A Power BI analytics project exploring water access, water quality, and service delivery challenges across the fictional nation of Maji Ndogo. Built using the ALX Data Analytics curriculum's "Maji Ndogo Summary" dataset, this dashboard turns raw water-source records into actionable insights for infrastructure planning and resource allocation.

A Power BI analytics project exploring water access, water quality, and service delivery challenges across the fictional nation of Maji Ndogo. Built using the ALX Data Analytics curriculum's "Maji Ndogo Summary" dataset, this dashboard turns raw water-source records into actionable insights for infrastructure planning and resource allocation.



📖 Overview

Maji Ndogo ("Small Waters/little water" in Swahili) is a fictional country used throughout the ALX Data Analytics curriculum to simulate real-world water infrastructure challenges. This project analyzes the Maji Ndogo Summary Dataset, a record of water sources, quality assessments, and population access across five provinces.

Dataset snapshot:

Attribute: Detail
Rows       -60,146
Columns    -23
Geographic scope- 5 provinces, multiple towns

Key variables; Water source type, contamination/pollutant levels, queue times, demographic indicators, population served

The goal of this dashboard is to apply data cleaning, exploratory data analysis (EDA), and visualization techniques to answer practical questions: Where are people underserved? Which water sources are most relied upon? How do queue times and demographics vary across the country? The resulting insights are intended to support data-driven decisions for improving water infrastructure.


📊 Dashboard Analytics

The report is organized into three interactive pages:

1. National Overview

A high-level snapshot of population distribution and water source reliance across the entire country, including the rural/urban split and the breakdown of people served by each water source type.

2. Maji Ndogo Provinces

A geographic (choropleth map) view showing the number of water sources per province, allowing users to filter and drill down into province-level infrastructure density.

3. Queue Analysis

A deep dive into the human cost of water collection — average wait times by day of the week, time-of-day patterns, gender/age composition of queues, and the relationship between crowd size and wait time at shared water sources.

All pages are fully interactive, with slicers and cross-filtering enabled so a selection on one visual updates the others.


📈 Key Visuals

Pie Chart


Number of people served by location type — splits the population into Rural vs. Urban segments.


Bar/Column Charts — Simple


Number of people per water source — ranks water source types (shared tap, well, tap in home, broken tap in home, river) by total population served.
Average time in queue by day of the week — highlights which days create the worst congestion at water points.


Bar Chart — Comparative


Rural/Urban human population distribution — a horizontal comparison of population counts across the two location types.
Gender distribution in water source queues per day — compares Child, Male, and Female composition side-by-side for each day of the week.


Choropleth (Geographic) Map


Number of water sources per province — shades each of Maji Ndogo's five provinces by relative water infrastructure density.


Line Chart


Queue average time by day of the week and hour of the day — tracks how wait times rise and fall throughout the day, separated by day-of-week series.


Scatter Plot


Average number of people in a queue vs. time in queue (shared water sources) — visualizes the correlation between crowd size and wait duration.



🔍 Key Insights & Findings


-63.85% of Maji Ndogo's population (≈18M people) lives in rural areas, compared to 36.15% (≈10M people) in urban areas.
-Shared taps are by far the most relied-upon water source nationally, serving roughly 12M people — more than double the next largest source (wells, ~4.8M).
-Only 7.55% of the rural population has a working tap inside their home, compared to a higher share in urban areas — underscoring a significant rural infrastructure gap.
-Wells serve substantially more people in rural areas than in urban areas, reflecting their role as a rural-specific water access solution.
-Hawassa has the fewest tap_in_home water sources of all five provinces (868), trailing well behind Amanzi (2,334), Sokoto (1,486), and Akatsi (1,281).
-Across the week, women consistently make up the largest share of queue composition, with female participation rising further on weekends relative to male and child participation.
-Saturday has by far the longest average queue time of any day (roughly 4x a typical weekday), suggesting weekend demand significantly outpaces available capacity.
-Queue times spike sharply during early morning (6–9am) and early evening (4–7pm) hours on weekdays, while Saturday maintains high queue times throughout the entire day.
-There is a strong positive correlation between the number of people in a queue and the time spent waiting — as crowd size approaches ~3,500–4,000 people, average wait times climb toward 500+ minutes.
-Amanzi stands out as the province that has made the most progress toward gender equality in water access.



🛠️ Tools & Technologies


Power BI Desktop — report design, data modeling, and visualization
Power Query (M) — data cleaning and transformation
DAX (Data Analysis Expressions) — calculated measures and columns (e.g., percentage-of-total and aggregation measures)
Maji Ndogo Summary Dataset — source data from the ALX Data Analytics curriculum



🚀 How to Use


Clone or download this repository:


bash   git clone https://github.com/<your-username>/<your-repo-name>.git


Open the .pbix file in Power BI Desktop (download Power BI Desktop free from Microsoft if you don't have it installed).
Refresh the data (Home → Refresh) if prompted, especially if you've relinked the source dataset to your own copy.
Explore the report:

Use the page navigation tabs to move between National, Provinces, and Queue Analysis views.
Click on any bar, slice, or map region to cross-filter the rest of the page.
Hover over visuals to see detailed tooltips.



(Optional) Modify or extend the report — add your own measures, pages, or visuals using the included dataset.



📁 Project Structure

maji-ndogo-water-dashboard/
│
├── README.md                     # Project documentation (this file)
├── Maji_Ndogo_Dashboard.pbix      # Power BI report file
├── data/
│   └── md_water_services.csv     # Source dataset (or link/instructions if too large for GitHub)
├── assets/
│   ├── national_overview.png     # Dashboard screenshots used in this README
│   ├── province_map.png
│   └── queue_analysis.png
└── docs/
    └── data_dictionary.md        # Column descriptions for the dataset (optional)


💡 Tip: If your .pbix file or dataset exceeds GitHub's file size limits, consider using Git LFS or linking to an external download (Google Drive, OneDrive, etc.) in this section.




👤 Author / Developer

Paul Kimaili | Data Analyst/Scientist | Data Engineer
📧 pkimaili2@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/paul-kimaili964/ 
· Github: [GitHub](https://github.com/Paulkimaili) 
· Portfolio: https://sites.google.com/d/10x_PV0wTMZdghMcV0ROsTVTYH6ZzsIuG/p/1GzxJS75XEbeo7YUYw7irzrApzcxIqy8Z/edit


🙏 Acknowledgments


ALX Africa — for the Data Analytics curriculum and the Maji Ndogo case study dataset
The broader Power BI and data analytics community for inspiration on dashboard design best practices



⭐ Support This Project

If you found this project worthwhile, please consider starring the repo — it helps others discover this work and motivates further projects like this one!
