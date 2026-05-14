# HVAC Load & Equipment Selector

An engineering-focused HVAC calculation and equipment screening tool for preliminary design, load estimation, and equipment selection.  
This project is built to support mechanical engineers, MEP designers, and HVAC practitioners who need a structured way to estimate building cooling/heating requirements, size major HVAC components, and compare candidate equipment based on calculated design conditions.

The tool is intended to reduce manual spreadsheet work and make HVAC design more reproducible, traceable, and easier to review. It consolidates core HVAC calculations into a single workflow, from thermal load estimation to equipment matching and selection logic.

---

## Project Purpose

HVAC system sizing is often done using scattered spreadsheets, manual formulas, and disconnected vendor catalogs. That makes design review slow, inconsistent, and difficult to audit.

This project addresses that problem by providing a calculation and selection framework that can:

- estimate room or zone cooling/heating loads,
- determine supply air requirements,
- evaluate airflow and capacity needs,
- screen HVAC equipment candidates,
- and generate a structured output for design comparison.

The final goal is to create a practical engineering utility for early-stage HVAC design, equipment screening, and load-based selection.

---

## Scope of Calculation

This project is designed to support the main calculation blocks commonly used in HVAC design and equipment selection.

### 1. Cooling Load Calculation
The tool can handle the main contributors to cooling load, including:

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

### 2. Heating Load Calculation
The tool can also estimate heating demand using the major heat loss terms, such as:

- transmission loss through building envelope,
- infiltration heat loss,
- ventilation heating load,
- zone or room heating demand.

### 3. Airflow Requirement Calculation
The project supports airflow sizing based on the calculated load and design assumptions, including:

- supply air volume requirement,
- return air estimation,
- outdoor air fraction,
- recirculation ratio,
- minimum airflow check,
- airflow balance logic.

### 4. Psychrometric and Airside Logic
To support HVAC design decisions, the tool can be extended or configured to handle:

- dry-bulb temperature,
- wet-bulb temperature,
- humidity ratio,
- relative humidity,
- enthalpy,
- sensible heat ratio,
- supply air condition selection,
- coil leaving air condition logic.

### 5. Equipment Selection Logic
The selector is intended to compare the load and airflow result against available HVAC equipment options such as:

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

The equipment selection step checks whether the candidate unit can satisfy:

- total capacity,
- sensible capacity,
- airflow requirement,
- pressure drop allowance,
- temperature difference,
- part-load suitability,
- and operational feasibility.

---

## Engineering Inputs

The tool is designed around practical HVAC design inputs such as:

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

The project is designed to work with the main HVAC system elements used in design and selection:

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

The tool is intended to produce outputs such as:

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

The goal is not only to calculate loads, but also to create a reusable HVAC engineering workflow that can be used for:

- concept design,
- preliminary sizing,
- equipment screening,
- design comparison,
- and engineering documentation.

This repository focuses on the logic behind HVAC selection, calculation transparency, and practical design use.

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
