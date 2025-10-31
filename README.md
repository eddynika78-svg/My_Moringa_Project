# My_Moringa_Project
# Airline Accident Risk Analysis — Phase 1 Data Science Project

## Student Information
- **Name:** Eddy Wiwatsu  
- **GitHub Username:** eddynika78-svg  
- **Institution:** Moringa School  
- **Project:** End of Phase 1 Data Science Project

---

## Project Overview
This project analyzes patterns in airline accidents to understand safety performance across different aircraft makes and models.  
The goal is to identify which aircraft types have historically recorded the **lowest and highest risk levels**, using available accident data.

---

## Objectives
1. Load and clean the dataset (`airline_accidents.csv`)
2. Explore trends over time (incidents, fatalities, serious injuries)
3. Identify the safest aircraft makes and models
4. Compute a **risk score** combining incident rate and severity
5. Visualize and summarize key findings

---

## Dataset Description
The dataset `airline_accidents.csv` contains historical records of airline accidents.  
Main columns include:
- **Date** – Date of the accident  
- **Location** – Where the accident occurred  
- **Make & Model** – Aircraft type  
- **Operator** – Airline company  
- **Aboard / Fatalities / Serious Injuries** – Key numerical indicators  
- **Summary** – Brief description of the incident  

---

## Tools and Technologies
- **Language:** Python 3  
- **IDE:** Jupyter Notebook  
- **Libraries Used:**
  - `pandas` – Data manipulation  
  - `numpy` – Numerical computations  
  - `matplotlib`, `seaborn` – Data visualization  
  - `datetime` – Date handling  

---

## Key Analysis Steps
1. **Data Loading and Cleaning**
   - Removed missing or irrelevant values
   - Standardized column names and types  
   - Extracted `Year` from accident dates  

2. **Exploratory Data Analysis (EDA)**
   - Distribution of accidents per year  
   - Fatalities and serious injuries over time  
   - Most frequent aircraft makes/models  

3. **Feature Engineering**
   - Aggregated statistics by aircraft `Make` and `Model`
   - Calculated a **Risk Score** using:
     \[
     \text{Risk Score} = \text{Incidents} + 0.5(\text{Fatalities}) + 0.3(\text{Serious Injuries})
     \]

4. **Visualization**
   - Top 10 lowest risk aircraft types  
   - Trends of total incidents by year  
   - Boxplot comparing risk scores across aircraft makes  

5. **Results Export**
   - Saved outputs in `/outputs/` folder  
   - Key file: `aggregated_risk_by_make_model.csv`

---

## Key Insights
- Aircraft models such as **Boeing 737** and **Airbus A320** appear frequently due to their large operational volume, not necessarily poor safety.  
- A few smaller models had high risk scores relative to their lower flight counts.  
- The **risk scores decreased over the years**, showing improved aviation safety globally.  

---

## Conclusions
- Historical accident data can highlight trends in safety improvement.
- Standardized data cleaning and aggregation techniques can support aviation risk assessment.
- Visualization makes interpretation of large datasets simpler and more actionable.




