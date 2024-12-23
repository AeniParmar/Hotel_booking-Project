# **Hotel Bookings Data Analysis Project**  

## **Project Overview**  
This project involves exploratory data analysis (EDA) on a hotel bookings dataset. The analysis aims to uncover insights related to reservation status, cancellation trends, country-wise cancellations, seasonal variations, and other factors impacting hotel reservations. The visualizations provide a clear understanding of patterns and anomalies in the data.  

---

## **Dataset Information**  

### **File Used**  
- **hotel_bookings.csv**: Contains data on hotel bookings, including customer demographics, reservation details, and booking status.  

### **Key Features**  
- `is_canceled`: Indicates whether a booking was canceled.  
- `hotel`: Type of hotel (Resort Hotel or City Hotel).  
- `adr`: Average Daily Rate per customer.  
- `reservation_status_date`: Date of the booking status update.  
- `market_segment`: Segment through which the booking was made.  
- `country`: Guest's country of origin.  

---

## **Libraries Used**  
- **Pandas**: For data manipulation and analysis.  
- **Matplotlib**: For creating static visualizations.  
- **Seaborn**: For statistical data visualization.  
- **Warnings**: To suppress warnings during execution.  

---

## **Steps Performed**  

### **1. Data Preprocessing**  
- Loaded the dataset and inspected its structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.columns`.  
- Converted `reservation_status_date` into a datetime format.  
- Identified and handled missing values:  
  - Dropped the `company` and `agent` columns due to a large number of missing values.  
  - Removed rows with missing values using `dropna()`.  
- Filtered out outliers in the `adr` column to keep values below 5000.  

### **2. Exploratory Data Analysis**  
- **Reservation Status**:  
  - Bar chart showing the distribution of canceled and non-canceled bookings.  
- **Reservation by Hotel Type**:  
  - Analyzed reservation and cancellation counts for Resort Hotel and City Hotel.  
- **Average Daily Rate (ADR)**:  
  - Plotted trends in ADR over time for both Resort Hotel and City Hotel.  
  - Compared ADR for canceled and non-canceled bookings.  
- **Monthly Reservation Trends**:  
  - Count plot displaying the number of reservations (canceled and non-canceled) across months.  
  - Analyzed monthly ADR for canceled bookings.  
- **Country-Wise Cancellations**:  
  - Pie chart highlighting the top 10 countries with the highest cancellation rates.  
- **Market Segment Analysis**:  
  - Distribution and proportions of bookings across various market segments.  

---

## **Key Insights**  
1. **Cancellations**:  
   - A significant proportion of bookings are canceled.  
   - Resort Hotels have a slightly higher cancellation rate than City Hotels.  
2. **Seasonal Trends**:  
   - Booking cancellations and ADR fluctuate across months, with notable peaks in certain periods.  
3. **Country Trends**:  
   - Most cancellations are concentrated in specific countries, with a few contributing disproportionately.  
4. **Market Segments**:  
   - Certain market segments dominate the booking data, with variations in cancellation tendencies.  

---

## **Visualizations Created**  
1. Bar chart for reservation status distribution.  
2. Count plot for reservation status by hotel type.  
3. Line plot showing ADR trends for Resort and City Hotels.  
4. Pie chart for top 10 countries with the highest cancellation rates.  
5. Count plot for monthly reservation status trends.  
6. Bar plot showing monthly ADR for canceled bookings.  

---

## **How to Run the Code**  

1. **Dependencies**  
   - Install necessary libraries using the following command:  
     ```bash  
     pip install pandas matplotlib seaborn  
     ```  

2. **Dataset Setup**  
   - Ensure the dataset file (`hotel_bookings 2.csv`) is in the same directory as the script.  

3. **Execution**  
   - Run the script in a Jupyter Notebook or any Python IDE to generate the analysis and visualizations.  

---

## **Future Scope**  
1. **Advanced Modeling**: Build predictive models to estimate cancellation probabilities.  
2. **Additional Features**: Explore other factors like lead time and special requests.  
3. **Interactive Dashboard**: Create a dashboard using tools like Tableau or Power BI for dynamic exploration.  

---
