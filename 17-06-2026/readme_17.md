Day 17 – Fuel Analytics Dashboard
Overview
This project is part of a 30‑day data challenge. On Day 17, I built an interactive, self‑contained HTML dashboard that analyses vehicle fuel data from a CSV file. The dashboard is designed for a data analyst to quickly compare fuel types, understand cost/CO₂ trade‑offs, and evaluate the E85 paradox – all with pure SVG visualisations and glass‑morphism styling.

Data Source
The CSV file (day17_e85_dataset_optimised.csv) contains 52 records of real‑world vehicle trips. Each row includes:

Column	Description
Fuel_Type	Petrol (E20), Diesel, CNG, Electric (EV), E85 (Flex‑Fuel)
Vehicle_Age_yrs	Age of the vehicle in years
Distance_km	Distance covered in kilometres
Fuel_Cost_INR	Total fuel cost for the trip (₹)
CO2_emitted_kg	CO₂ emissions in kilograms
Maintenance_Cost_INR	Maintenance cost for the trip (₹)
Refuel_Recharge_time_min	Time taken to refuel/recharge (minutes)
Fuel_Price_per_unit_INR	Price per unit of fuel (₹/kg, ₹/L, or ₹/kWh)
Typical_Mileage	Fuel economy (km/kg, km/L, or km/kWh)
Dashboard Features
The dashboard is a single HTML file with inline CSS and JavaScript – no external libraries or CDN. It delivers:

1. Header
Vehicle model (Toyota Camry)

Selected fuel (Petrol E20)

Vehicle age (3 years)

Monthly usage (1,500 km/mo)

2. KPI Cards
Five key performance indicators:

Your fuel cost per kilometre

E85 cost per kilometre

E85 premium (or saving) vs. Petrol

Break‑even price for E85

Your estimated monthly fuel cost

3. Bar Chart – Cost per km by Fuel
Compares the average cost per kilometre for all five fuel types. The user’s fuel is highlighted with a gold dashed border.

4. Doughnut Chart – CO₂ per km by Fuel
Shows the proportional CO₂ emissions per kilometre for each fuel. Hover over any segment to see the exact value.

5. Line Chart – Cost/km vs. Vehicle Age
Plots cost per kilometre against vehicle age (0–12 years) for each fuel. A vertical gold line marks the user’s vehicle age (3 years). Points are drawn from both the raw data and the age‑bucket aggregates.

6. E85 Gauge & Verdict
Animated gauge shows the E85 Score / 10 (based on cost, CO₂, refuel time, and maintenance).

A one‑sentence verdict explains the score.

7. E85 Paradox Panel
Displays three critical figures:

Pump saving – percentage saved at the pump (vs. Petrol)

Running penalty – extra cost per kilometre (vs. Petrol)

Break‑even price – the E85 price that would make it equally cost‑effective

8. Fuel Cards
Each fuel type is presented in a card with:

Pros (✅) and cons (❌)

Best‑use recommendation (🚗)

The user’s fuel card glows for quick identification.

Metrics Computed (Grouped by Fuel_Type)
From the raw CSV, the dashboard calculates:

Metric	Formula
Avg Cost/km	Fuel_Cost_INR ÷ Distance_km
Avg CO₂/km	CO2_emitted_kg ÷ Distance_km
Avg Maintenance/km	Maintenance_Cost_INR ÷ Distance_km
Avg Refuel Time	Average of Refuel_Recharge_time_min
Age Buckets
Vehicles are grouped into:

New (0–2 years)

Mid‑life (3–5 years)

Aged (6–9 years)

Old (10+ years)

For each bucket, we compute Cost/km and Maintenance/km, and the line chart uses these aggregates alongside raw data points.

E85 Score (out of 10)
The score is a weighted composite designed to give a holistic view of E85 performance:

Component	Weight	Rationale
Cost/km	4 pts	Most important for everyday users
CO₂/km	3 pts	Environmental impact
Refuel time	2 pts	Convenience factor
Maintenance/km	1 pt	Long‑term ownership cost
Each component is normalised across all fuel types, so the score reflects E85’s relative standing.

How to Use
Open the HTML file in any modern browser.

The dashboard loads automatically – all data is embedded in the script.

Hover over the doughnut chart to see exact CO₂ values.

The gauge animates on load; refresh to see the animation again.

All charts are responsive and work from 375px to 1440px+.

Technical Stack
HTML5 – semantic structure

CSS3 – custom properties, glass‑morphism, flex/grid layouts

Vanilla JavaScript – no frameworks, all computation and rendering done in the browser

SVG – all charts are drawn natively; no canvas or external charting libraries

Data embedded – the CSV is parsed directly inside the script

File Structure
text
day17/
├── day17_e85_dataset_optimised.csv   # raw data
├── index.html                        # standalone dashboard (all CSS/JS inside)
└── README.md                         # this file
Future Enhancements
Allow the user to input their own vehicle details (fuel, age, km/mo) via a form.

Add drill‑down to individual trip records.

Export charts as PNG.

Compare two fuels side‑by‑side with dynamic selection.

Author
Part of the 30‑day data challenge – a daily exercise in data analysis, visualisation, and storytelling.