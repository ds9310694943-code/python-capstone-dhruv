# python-capstone-dhruv
<img width="1907" height="965" alt="Screenshot 2025-12-06 120309" src="https://github.com/user-attachments/assets/21a53be0-2654-4b17-881e-2e7218645173" />
🎯 Objective

The goal of this project is to analyze electricity usage across multiple campus buildings and generate clear, actionable insights for improving energy efficiency. This project delivers:

📊 A unified dataset combining all building meter readings

📈 Daily and weekly consumption trends

🏢 Building-wise performance summaries

🖼️ A visual dashboard showing key patterns

📝 A text-based executive summary for decision-makers

📁 Dataset Source

All datasets are stored as individual CSV files in the /data folder. Each CSV represents one building’s electricity meter readings.

Example structure:

Timestamp,kWh 2024-01-01 00:00,10 2024-01-01 01:00,12 ...

🔧 During data ingestion, every file is automatically labeled with the building name (derived from the filename).

🔧 Methodology

The project follows a complete data-processing pipeline:

1️⃣ Data Ingestion

📥 Load all .csv files from /data

🧹 Remove missing or corrupted rows

🏷️ Add building names automatically

2️⃣ Data Processing & Aggregation

🔄 Convert timestamps into datetime format

🧮 Compute:

Daily totals

Weekly totals

Building-wise stats (mean, min, max, total)

3️⃣ Object-Oriented Modeling (OOP)

🧱 Classes implemented:

MeterReading

Building

BuildingManager

🔗 Each reading is stored as an object inside its building

4️⃣ Visualization

📊 A dashboard using Matplotlib featuring:

Line graph → daily consumption

Bar chart → weekly average per building

Scatter plot → energy usage over time

5️⃣ Output Generation

💾 cleaned_energy_data.csv

📄 building_summary.csv

📝 summary.txt (executive report)

🖼️ dashboard.png

💡 Insights

From the sample dataset used:

🏆 Building C had the highest total electricity consumption

⚡ Peak usage typically occurred during early hours

📉 Daily usage patterns were consistent across buildings

📊 Weekly averages highlighted which buildings fluctuate vs stay stable

These insights can help administrators:

🔍 Identify inefficient buildings

🕒 Predict peak demand periods

🌱 Support sustainability and energy-saving strategies

🛠️ Prioritize buildings for upgrades or audits
