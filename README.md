# Real-Time Electricity Data Pipeline

An end-to-end data engineering pipeline that retrieves electricity generation and emissions data from the OpenElectricity API, processes it, streams it via MQTT, and visualizes it on a live interactive dashboard.

## Overview

This project demonstrates a real-time data engineering workflow including:

- Data retrieval from REST APIs
- Data cleaning and transformation
- Stream processing using MQTT
- Real-time visualization using Plotly

The system simulates a live data stream of electricity generation across Australia's National Electricity Market (NEM).

---

## Architecture

1. **Data Ingestion**
   - Retrieve facility power generation and CO₂ emissions data from the OpenElectricity API.

2. **Data Processing**
   - Clean and merge power, emissions, facility, and market data.

3. **Streaming Pipeline**
   - Publish data as MQTT messages with event-time ordering.

4. **Real-Time Dashboard**
   - Subscribe to the MQTT stream and visualize facility-level electricity generation and emissions on an interactive map.

---

## Technologies Used

- Python
- Pandas
- MQTT
- Plotly
- REST APIs
- Jupyter Notebook

---

## Repository Structure



---

## Dashboard Features

- Live electricity generation monitoring
- Facility-level emissions tracking
- Interactive map visualization
- Toggle between power output and emissions view
- Real-time updates from streaming data

---

## Example Visualization

(Add screenshots here)

---

## Project Report

The full project report can be found here:

[Project Report](docs/Project_Report.pdf)

---

## Author

Sanskar Agarwal
