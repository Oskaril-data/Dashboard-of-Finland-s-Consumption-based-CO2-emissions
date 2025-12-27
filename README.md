
# 🇫🇮 Finland Carbon Transition & Policy Simulator

An interactive Excel-based analytical tool designed to visualize Finland's **Consumption-Based Emissions (CBE)** and simulate the impact of environmental policies on achieving a sustainable carbon footprint.

---

## 📊 Project Overview
This dashboard allows users to step into "Dictator Mode" to influence Finland's environmental path. While most national reports focus on production emissions, this project tracks **what Finns actually consume**, including imported goods and international aviation. The ultimate goal is to see if policy changes can bring the average footprint down to the IPCC-recommended level of **2,000 kg CO2 per capita**.

---

## 🚀 Key Features
* **Interactive Policy Simulator:** Toggle real-world policies (e.g., dietary shifts, aviation taxes) using Excel Form Controls.
* **Dynamic Goal Tracking:** Real-time feedback on how close your policies bring Finland to the "Sustainability Target."
* **Integrated Carbon Sinks:** Accounts for LULUCF (Land Use, Land-Use Change, and Forestry) data to show the true net impact.

---

## 🛠️ Technical Workflow (ETL & Analysis)

### 1. Data Ingestion & Cleaning (Power Query)
* **Source:** Global emissions data from *Our World in Data (OWID)*.
* **Process:** Used **Power Query** to isolate Finland, handle missing values, and transform "dirty" source data into a clean, analysis-ready format.

### 2. Data Mashup (StatFi Integration)
* **Source:** *Statistics Finland (StatFi)*.
* **Reasoning:** Standard CBE data often misses the land-use sector. I manually integrated **LULUCF** data to provide a more accurate picture of Finland’s net carbon balance.

### 3. Calculation Engine
* **Advanced Logic:** Built using weighted averages and dynamic references.
* **Formulas:** Leveraged `XLOOKUP`, `IF-logic`, and **Dynamic Arrays** to ensure the dashboard updates instantly without lag.

---

## 🕹️ "Dictator Mode" Policies
The simulation includes several key levers:
* **Aviation Reform:** Captures international flight emissions, which are often "hidden" in standard national reports.
* **Dietary Shift & Reforestation:** Simulates a move to plant-based diets. The model assumes that liberated agricultural land is **reforested**, increasing carbon sequestration over time.
* **Energy & Transport:** Accelerating the electrification of the private car fleet.

> **Note:** Policy impact coefficients are coarse estimates based on environmental reports (SYKE/Luke) and are intended for illustrative proof-of-concept purposes.

---

## 📈 Technical Skills Demonstrated
| Skill | Implementation |
| :--- | :--- |
| **ETL** | Power Query (Merging OWID & StatFi datasets) |
| **Data Modeling** | Creating relationships between consumption data and LULUCF sinks |
| **UX/UI Design** | Building a clean, professional "Our World in Data" style interface |
| **Analysis** | "What-If" analysis and goal-seeking logic |

---

## 🔮 Future Roadmap
* **Carbon Sink Maximization:** Adding a toggle to simulate restoring Finland’s sinks to their historical peaks (~46 Mt).
* **Live API Connection:** Replacing CSV imports with live Power Query web connections.
* **Socio-Economic Layer:** Calculating how policies affect different income deciles (Social Justice focus).

---

*This project was developed as a rapid prototype to demonstrate advanced data manipulation and visualization capabilities in Excel.*
