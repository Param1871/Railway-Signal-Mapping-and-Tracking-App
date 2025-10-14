Railway Signal Mapping and Tracking App
========================================

Overview
--------
The Railway Signal Mapping and Tracking App is a desktop application developed in Python to address the problem of inconsistent cellular network coverage during train journeys across India. It integrates real-world geographic data with a dynamic simulation model to predict and visualize network stability for major Internet Service Providers (ISPs) like Jio, Airtel, Vodafone Idea, and BSNL.

This tool helps commuters and logistics operators analyze signal performance, plan routes, and select the best ISP based on coverage and speed statistics.

Key Technologies Used
----------------------
- GUI: Tkinter & ttk — for building the interactive desktop interface.
- Geospatial: Folium, webbrowser, os — for creating and viewing interactive signal maps.
- Data Science: Pandas, NumPy, JSON — for data handling, route simulation, and calculations.
- Visualization: Matplotlib — for generating comparative charts and analytics.

Features
--------
1. Route Search & Selection
   - Users can choose source and destination stations.
   - The system lists available direct trains between stations.
   - Selection triggers route simulation and ISP analysis.

2. Comparative Data & Analytics
   - Simulates ISP signal strength (kbps) along each route segment.
   - Displays average, maximum, and minimum signal speed per ISP.
   - Identifies weak signal zones near stations.

3. Visualization & Reporting
   - Bar and Pie charts compare network performance.
   - Heatmap on interactive map (Folium) shows route signal strength by color:
     - Green: Good Signal
     - Yellow: Average Signal
     - Red: Weak Signal
   - Detailed station-by-station schedule view.

Installation
------------
Requirements:
- Python 3.8 or above
- Dependencies: numpy, pandas, folium, matplotlib, tk

Installation Command:
pip install numpy pandas folium matplotlib tk

Running the Application:
1. Place `stations.json`, `trains.json`, and `schedules.json` in the same folder as `app.py`.
2. Run the app using:
   python app.py

Future Enhancements
-------------------
- Integration with real-time mobile network APIs for live data.
- Web version using Flask or Django for remote access.
- Time-based signal quality analysis by train schedule.
- Advanced algorithm refinement for smoother signal predictions.
