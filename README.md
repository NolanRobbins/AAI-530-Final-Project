# AAI 530 Final Project

## Purpose

This project proposes a manufacturing process monitoring & predictive maintenance system for CNC milling centers that (1) detects anomalous machining behavior in real time, (2) predicts near-term vibration escalation (early warning), and (3) surfaces
status/alerts in an operator dashboard.

The system will produce actionable alerts (anomaly classification) and forecasts (short-horizon vibration trend predictions) to minimize downtime and avoid part scrap.

## Primary Users

- shop-floor engineers
- predictive-maintenance teams
- production managers.

## Dataset

[Bosch CNC Machining Dataset](https://archive.ics.uci.edu/dataset/752/bosch+cnc+machining+dataset)  
[Dataset GitHub repo](https://github.com/boschresearch/CNC_Machining)
    - Components of the dataset github repo were copied into this project for ease of access.

- Tri-axial acceleration measured by a Bosch CISS accelerometer mounted inside brownfield CNC milling machines (X, Y, Z axes), sampled at 2 kHz. Data was captured in an edge-to-cloud setup during real production over multiple 6-month timeframes (Oct 2018 – Aug 2021), and manually annotated as “good” (normal) or “bad” (anomalous).
- How many observations are in the dataset?
- 2700 time-series instances
- Vibration time series: tri-axial accelerometer channels (X, Y, Z) — high-frequency
(2 kHz)
- Metadata per file: machine number (M01–M03), process id (OP00–OP14),
timeframe (labeled by month/year), example id, and manual label (“good”/“bad”)
