# Real-Time Electricity Data Pipeline

An end-to-end data engineering pipeline that retrieves electricity generation and emissions data from the OpenElectricity API, processes it, streams it via MQTT, and visualizes it on a live interactive dashboard.

*Note: For convenience, a compressed dataset (`power_emission.csv.zip`) is provided in this repository to allow users to test the pipeline without repeating the full data ingestion process. Please unzip the file to obtain `power_emission.csv` before running the notebooks.*

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

```
real-time-electricity-data-pipeline
│
├── INGEST_CLEAN_PUBLISH.ipynb
│   Data ingestion, cleaning, transformation, and MQTT publishing pipeline
│
├── SUBSCRIBE_DECODE_VISUALIZE.ipynb
│   MQTT subscriber and real-time dashboard visualization
│
├── A1_Dataset.csv
│   Facility metadata used for location and facility mapping
│
├── power_emission.csv.zip
│   Cleaned dataset containing integrated power and emissions data
│
├── requirements.txt
│   Python dependencies required to run the project
│
├── README.md
│   Project overview, architecture, and usage instructions
│
└── docs
    └── project_report.pdf
        Full project report describing methodology and system design
```

---

## Dashboard Features

- Live electricity generation monitoring
- Facility-level emissions tracking
- Interactive map visualization
- Toggle between power output and emissions view
- Real-time updates from streaming data

---

## Example Visualization

<img width="894" height="596" alt="image" src="https://github.com/user-attachments/assets/e62d4f66-bc65-4995-a5f4-30d9b147b215" />

<img width="894" height="596" alt="image" src="https://github.com/user-attachments/assets/617581d8-4419-439c-ac17-f510a91b7a88" />

<img width="894" height="596" alt="image" src="https://github.com/user-attachments/assets/f1d4632f-3ead-440c-874e-a000d5ff5b01" />

<img width="894" height="596" alt="image" src="https://github.com/user-attachments/assets/06daef92-fcb9-4e5b-88d2-92f860169cae" />



---

## Project Report

The full project report can be found here:

[Project Report](docs/Project_Report.pdf)

---

## Author

Sanskar Agarwal
