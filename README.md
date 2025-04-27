# Aircraft Risk Analysis.

## Project Overview

Our company is diversifying its portfolio by entering the aviation industry. To ensure a safe and successful entry, the leadership team is exploring which aircraft models are lowest risk for purchase and operation. This project aims to analyze historical aviation accident data to determine which aircraft present the **lowest operational risk**, enabling data-driven acquisition decisions for both **commercial** and **private enterprise** use cases.

![aircraft](images\aircraft.jpg)

Photo by <a href="https://media.istockphoto.com/id/1455888136/photo/luxury-private-jet.jpg?s=612x612&w=0&k=20&c=jtAd4usrdWHczYRQtc4WfSbBjhU2xB7gNv13fgLrz_k=">dicus63</a> on <a href="https://media.istockphoto.com/id/1455888136/photo/luxury-private-jet.jpg?s=612x612&w=0&k=20&c=jtAd4usrdWHczYRQtc4WfSbBjhU2xB7gNv13fgLrz_k=">Istock</a>

## Business Understanding

### Problem Statement
The company is planning to enter the aviation industry but lacks expertise in identifying safe and reliable aircraft. The task is analyzing aviation incident data to determine which aircraft are the **lowest risk**. Your insights will help the aviation division make informed purchasing decisions.

### Objectives
- Identify aircraft models with **the fewest or least severe incidents**.
- Understand patterns and risk factors across different aircraft.


## Data Understanding
The dataset contains historical records of aviation incidents and accidents, including:
- Aircraft information (Make, Model, Engine Type)
- Incident characteristics (Injury Severity, Damage, Weather Conditions)
- Operational context (Purpose of Flight, Number of Engines)

## Exploring the Aviation Dataset
First, I imported the essential libraries
I explored the size and structure of the data by:

- Checking its shape with aviation_df.shape to see how many rows and columns we have.

- Viewing detailed column info (data types, non-null counts) using aviation_df.info().

## Data Cleaning Process
- First I checked an overview of the missing values and did the data cleaning on a copy of the dataset.
- dropped columns which were not relevant to the dataset.
- filled the categorical columns with "Unknown" as placeholders
- dropped rows with missing values in "Event.Date" and "Accident.Number"

After the cleaning process:

- I now have 88,777 complete entries.

- There are 21 well-organized columns capturing critical details about each event.

- All missing values in important fields like Event.Date, Accident.Number, Country, and Location have been handled.

- Non-critical missing information (like injury severity or weather conditions) has been clearly marked as 'Unknown' instead of being left blank.

##  EDA
The EDA process focuses on understanding the structure, distribution, and patterns within the dataset. The 
The following are my EDA questions:
- Top 10 Aircraft Models and Makes involved in Accidents
- The top 10 Deadliest Aircraft Models and Make
- Most dangerous flight phases(based on fatalities)
- whether there is a correlation between number of engines and Total fatal injuries


## Analysis Tools & Techniques
- Jupyter Notebook: Used for data cleaning, exploratory analysis, and visualization.

- Tableau: Used for advanced data visualization and dashboard creation for stakeholders. The link to my dashboard is: https://public.tableau.com/app/profile/edna.maina/viz/ProjeectDashboard/Dashboard1?publish=yes

Python Libraries:

- Pandas (data manipulation)

- Matplotlib & Seaborn (data visualization)

- NumPy (numerical operations)

