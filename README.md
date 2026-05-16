# HVAC Load & Equipment Selector

The purpose is to have a practical HVAC engineering tool for estimating building loads, checking airflow requirements, and screening equipment against calculated design conditions. Instead of spreading the work across disconnected spreadsheets and manual checks, this project keeps the calculation flow in one place.

---

## Project Purpose

HVAC sizing is often handled through scattered spreadsheets, hand calculations, and vendor catalogs that are not always easy to trace or compare. That makes review slower and creates room for inconsistency.

This project brings the main steps into a single workflow so the design process is easier to follow and verify. It is meant to:

- estimate room or zone cooling and heating loads,
- determine supply air requirements,
- evaluate airflow and capacity needs,
- screen HVAC equipment candidates,
- and produce a structured output for design comparison.

The goal is to make early-stage HVAC design more practical, reproducible, and easier to audit.

---

## Scope of Calculation

The workbook and future dashboard are built around the calculation blocks that usually appear in HVAC design and equipment selection.

### Cooling Load Calculation
The tool covers the main contributors to cooling load, including:

- sensible heat gain,
- latent heat gain,
- internal heat gain,
- envelope heat gain,
- ventilation load,
- infiltration load,
- equipment load,
- lighting load,
- occupancy load,
- solar gain contribution.

### Heating Load Calculation
The tool can also estimate heating demand using the main heat loss terms, such as:

- transmission loss through the building envelope,
- infiltration heat loss,
- ventilation heating load,
- zone or room heating demand.

### Airflow Requirement Calculation
Airflow sizing is based on the calculated load and design assumptions, including:

- supply air volume requirement,
- return air estimation,
- outdoor air fraction,
- recirculation ratio,
- minimum airflow check,
- airflow balance logic.

### Psychrometric and Airside Logic
The project can be extended to handle the air-side conditions commonly used in HVAC design, such as:

- dry-bulb temperature,
- wet-bulb temperature,
- humidity ratio,
- relative humidity,
- enthalpy,
- sensible heat ratio,
- supply air condition selection,
- coil leaving air condition logic.

### Equipment Selection Logic
The selector compares load and airflow results against common HVAC equipment options such as:

- Air Handling Unit (AHU),
- Fan Coil Unit (FCU),
- Package Unit,
- Split Unit / DX Unit,
- Chiller system,
- Cooling coil,
- Heating coil,
- Supply fan,
- Return fan,
- Exhaust fan,
- Fresh air unit / ventilation unit,
- Outdoor air handling section.

The selection step checks whether the candidate equipment can satisfy:

- total capacity,
- sensible capacity,
- airflow requirement,
- pressure drop allowance,
- temperature difference,
- part-load suitability,
- and operational feasibility.

---

## Engineering Inputs

The tool is designed around the inputs that are normally available during HVAC design, such as:

- room dimensions,
- building area and volume,
- occupancy density,
- lighting load,
- equipment load,
- internal heat sources,
- wall / roof / glass properties,
- outdoor design temperature,
- indoor design temperature,
- humidity condition,
- ventilation requirement,
- infiltration rate,
- desired supply air condition,
- equipment performance parameters.

---

## Equipment Categories Covered

The project is intended to work with the main HVAC system components used in design and selection:

- AHU
- FCU
- Split AC
- DX system
- Chiller
- Cooling coil
- Heating coil
- Supply fan
- Return fan
- Exhaust fan
- Fresh air unit
- Dampers
- Filters
- Diffusers
- Grilles
- Ductwork sections

---

## Expected Output

The tool is expected to produce outputs such as:

- calculated cooling load,
- calculated heating load,
- airflow requirement,
- selected equipment capacity,
- equipment suitability status,
- calculation summary,
- design assumptions,
- and comparison tables for alternative equipment.

---

## Project Goal

The goal is not only to calculate loads, but to build a reusable HVAC engineering workflow that can support:

- concept design,
- preliminary sizing,
- equipment screening,
- design comparison,
- and engineering documentation.

This repository focuses on calculation transparency, equipment selection logic, and practical HVAC design use.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Plotly
- Streamlit
- SQLite / CSV
- GitHub Pages for landing page
- Streamlit Community Cloud for demo deployment

---

## Repository Intent

This repository is meant to serve as:

- an HVAC engineering calculator,
- a design support tool,
- a portfolio project for mechanical engineering,
- and a foundation for a future interactive HVAC dashboard.

---

## Inspiration and Contribution

This project was inspired by the HVAC anomaly detection pipeline in [HVAC-Fault-Detection-with-Anomaly-Pipeline](https://github.com/shahabsalehi/HVAC-Fault-Detection-with-Anomaly-Pipeline).

I used that project as a reference for how an HVAC workflow can be organized clearly from data to output. Its dashboard and pipeline structure helped shape how I wanted this repository to feel: practical, traceable, and engineering-focused.

My contribution here is different. This repository is centered on HVAC load calculation and equipment selection, not fault detection. The goal is to support early design work by estimating loads, checking airflow needs, and comparing candidate equipment in one place.
