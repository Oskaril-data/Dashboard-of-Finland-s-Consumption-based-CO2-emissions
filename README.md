
Finland Carbon Transition & Policy Simulator

An interactive Excel-based analytical tool designed to visualize Finland's consumption-based CO2 emissions and simulate the impact of various environmental policies on achieving a sustainable carbon footprint.
Project Overview

This project provides a comprehensive look at Finland’s greenhouse gas emissions, moving beyond traditional production-based metrics to focus on Consumption-Based Emissions (CBE). The goal was to create a "Dictator Mode" simulator where users can implement various policies to see how they affect the journey toward the IPCC-recommended sustainable level of 2,000 kg CO2 per capita.
🛠️ Technical Workflow (ETL & Analysis)

    Data Ingestion & Cleaning (Power Query): * Extracted global emissions data from Our World in Data (OWID).

        Utilized Power Query to filter, transform, and isolate Finland’s specific data from the global dataset.

    Data Mashup (StatFi Integration): * Integrated official data from Statistics Finland (StatFi) regarding the LULUCF (Land Use, Land-Use Change, and Forestry) sector, as standard CBE data often overlooks these land-use impacts.

    Modeling & Visualization:

        Developed Pivot Tables and Dynamic Charts to visualize historical trends.

        Built a Calculation Engine that uses weighted averages to simulate the per capita impact of policy changes in real-time.

🕹️ Interactive Policy Simulator

The dashboard features an interactive policy panel using Excel Form Controls (Checkboxes). Users can toggle specific legislative actions, including:

    Aviation Reform: Includes the high-impact footprint of international flights, which are often excluded from national inventories but included in CBE.

    Dietary Shift: Simulates a transition toward plant-based diets. The logic assumes that reduced livestock demand frees up agricultural land for reforestation, thereby increasing long-term carbon sequestration.

    Transport & Housing: Toggles for accelerating the electrification of the national car fleet and improving energy efficiency in housing.

🧪 Methodology & Limitations

    Rapid Prototype: This project was developed as a proof of concept (within a few hours) to demonstrate advanced Excel capabilities.

    Policy Estimates: The coefficients used for policy impacts are coarse estimates based on environmental reports (e.g., SYKE/Luke) and are intended for illustrative purposes.

    Carbon Sinks: While historical LULUCF data is included in the background analysis, active simulation of "Carbon Sink Maximization" is currently a planned feature.

🚀 Future Roadmap

    Carbon Sink Maximization: Adding a toggle to simulate the restoration of Finland’s carbon sinks to their historical peak levels.

    Automated Data Pipelines: Connecting Power Query directly to StatFi and OWID APIs for "one-click" updates.
