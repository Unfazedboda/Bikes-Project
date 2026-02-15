[Project Title: London Bike Sharing Strategic Analysis]
📌 Project Overview
This project provides a comprehensive end-to-end analysis of London's bike-sharing system. It integrates a Python-driven ETL pipeline with an advanced Tableau dashboard to visualize how environmental variables like temperature, wind speed, and humidity influence urban mobility patterns.

The final deliverable is a high-performance, interactive dashboard that allows stakeholders to transition from high-level trends to granular hourly insights.

🛠️ Technical Implementation
1. Data Engineering (Python)
Before visualization, the raw data (17,000+ records) was processed using Python to ensure data integrity and usability:

Automated Retrieval: Leveraged the Kaggle API for programmatic data ingestion.

Data Transformation: * Mapped categorical integers to descriptive labels (e.g., Weather: "Clear", "Broken Clouds"; Seasons: "Spring", "Summer").

Normalized humidity values into percentage format.

Converted timestamps into standardized DateTime objects for time-series analysis.

Tools: Python, Pandas, Kaggle API.

2. Advanced Analytics (Tableau)
The dashboard utilizes complex Tableau features to provide a seamless user experience:

Dynamic Moving Averages: Implemented parameters that allow users to toggle between Daily, Weekly, or Monthly views and adjust the smoothing duration (e.g., 5-day vs. 50-day average).

Interactive Set Actions: Developed a "Drag-to-Select" feature on the timeline. Selecting a range on the main viz dynamically updates the KPIs and the Environmental Heatmap.

Viz-in-Tooltip: Integrated micro-charts within tooltips to show ridership by hour and weather condition without adding visual clutter to the main screen.

📊 Business Insights
Peak Commute Times: Analysis reveals significant spikes in ridership between 7:00 AM – 9:00 AM and 5:00 PM – 7:00 PM, indicating a heavy reliance on the system for commuting.

Weather Sensitivity: There is a strong correlation between "Feels Like" temperature and ridership; however, humidity levels above 80% result in a sharper decline in usage than moderate wind speeds.

Seasonal Trends: Summer months show the highest volume, but the moving average reveals that ridership is becoming increasingly resilient during shoulder seasons (Spring/Autumn).
