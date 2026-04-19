# Cognifyz_Railway-Data-Analysis
Data engineering assignment for Cognifyz Technologies involving data exploration, cleaning, transformation, analysis, and visualization.


## Project Overview
This project focuses on the exploration, cleaning, transformation, and analysis of a railway train dataset using Python-based data engineering techniques. The dataset contains information about train numbers, train names, source stations, destination stations, and operating days. The goal of this project is to extract meaningful insights and visualize patterns in train operations.

---

## Objectives
- Perform data exploration and inspect dataset structure  
- Handle missing values and clean the dataset  
- Apply data transformation and aggregation techniques  
- Analyze operational patterns across different days  
- Generate insights using visualizations  
- Create a report suitable for stakeholders  

---

## Tools & Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**

---

## Dataset Information
The dataset contains the following columns:

- `Train_No`
- `Train_Name`
- `Source_Station_Name`
- `Destination_Station_Name`
- `days`

### Key Observations
- Dataset contains **11,000+ records**
- Hundreds of unique source and destination stations
- Missing values were present in station names, train names, and days column

---

## Data Cleaning Steps
The following preprocessing steps were performed:

- Removed rows with missing **Source_Station_Name** or **Destination_Station_Name**
- Filled missing values:
  - `Train_Name` → **"Unknown"**
  - `days` → **"Not Available"**
- Standardized station names:
  - Converted all station names to **uppercase**
  - Removed extra spaces

---

## Data Transformation & Aggregation

### Data Filtering
- Implemented filtering to extract trains operating on specific days  
- Used mapping from short day formats (e.g., `MON`) to full day names (`Monday`)

### Grouping and Aggregation
- Grouped data by **Source_Station_Name** to count trains originating from each station
- Calculated **average trains per day per station**

### Data Enrichment
A new column `Day_Type` was added:

- **Weekday** → Monday to Friday  
- **Weekend** → Saturday and Sunday  

This improved analysis of train operations by category.

---

## Pattern Analysis

### Day-wise Distribution
- Analyzed distribution of train operations across all days
- Visualized using bar charts

**Insight:**  
Some days show higher train frequency, indicating peak demand.

### Route Analysis
- Grouped dataset by source and destination stations
- Identified top 10 most frequent routes

**Insight:**  
Certain routes occur repeatedly, indicating major travel corridors.

---

## Correlation & Insights

### Observations
- Train frequency differs across days of the week  
- Some stations act as major hubs with significantly higher train counts  
- A few routes dominate overall traffic  

### Recommendations
- Increase train frequency on high-demand days  
- Optimize scheduling on low-demand days  
- Improve infrastructure at high-traffic stations  
- Focus on improving high-frequency routes  

---

## Visualizations Created
The project includes the following visualizations:

- **Bar Chart:** Top 10 source stations by number of trains  
- **Bar Chart:** Day-wise distribution of trains  
- **Line Chart:** Weekly trend of train operations  
- **Heatmap:** Relationship between source stations and operating days  

These visualizations helped identify patterns and trends clearly.

---

## Conclusion
This project demonstrates:
- Data cleaning and preprocessing workflows  
- Aggregation and transformation for meaningful analysis  
- Pattern analysis in railway operations  
- Visualization techniques for clear reporting  

The insights can support better railway scheduling, resource allocation, and decision-making.

---

## References
- Python Documentation: https://www.python.org/doc/  
- Pandas Documentation: https://pandas.pydata.org/docs/  
- NumPy Documentation: https://numpy.org/doc/  
- Matplotlib Documentation: https://matplotlib.org/stable/contents.html  
- Seaborn Documentation: https://seaborn.pydata.org/  

---

## Author
**Srijita Mukherjee**  
Ref.: **CTI/A1/C326533**  
Submitted to: **Cognifyz Technologies**
```
