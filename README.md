# Patient Health Data Analysis – Tableau Project

This project analyzes patient health data using **Tableau**. It highlights missing values, visualizes patient conditions, and provides insights through interactive dashboards.

## Dataset

The dataset includes the following fields:

- **PatientID**: Unique identifier for each patient  
- **BloodPressure**: Patient's blood pressure readings  
- **Cholesterol**: Cholesterol levels  
- **Glucose**: Glucose levels  
- **Other fields**: (Add if any)

*The dataset is used to identify missing data and visualize the health status of patients.*

## Project Steps

1. **Data Import:** Load the dataset into Tableau.
2. **Sheet 1 – Overview:** Count of total patients and conditions.
3. **Sheet 2 – Condition Distribution:** Visualize the distribution of patients across conditions.
4. **Sheet 3 – Missing Data Highlight:**  
   - Created a **calculated field** to identify missing values:
     ```text
     IF ISNULL([BloodPressure]) OR ISNULL([Cholesterol]) OR ISNULL([Glucose]) 
     THEN "Missing" 
     ELSE "Complete" 
     END
     ```
   - Drag this field to **Color** to highlight patients with missing data.
5. **Dashboard Creation:** Combine all sheets into an interactive dashboard for quick insights.

## Insights

- Easily identify patients with incomplete data.  
- Monitor distributions of key health metrics.  
- Supports decision-making for further data collection or patient follow-up.

## Tools Used

- **Tableau Desktop** – For data visualization and dashboard creation

## How to Use

1. Open the Tableau workbook (`.twb` or `.twbx`) file.  
2. Interact with the dashboard to explore missing data and patient metrics.  
3. Filters and highlights are interactive to allow focused analysis.

