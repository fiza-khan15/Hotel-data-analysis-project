# Hotel Booking Cancellations Data Analysis

## 📌 Project Overview
This project explores and analyzes hotel booking data to uncover patterns in reservation status, cancellation trends, and customer behavior. The dataset contains details about reservations, hotels, booking status, market segments, and guest information.  

The analysis involves:
- Data cleaning and preprocessing  
- Handling missing values  
- Exploratory Data Analysis (EDA)  
- Visualizations of booking cancellations, ADR (Average Daily Rate), and market trends  
- Identifying patterns in cancellations across hotels, countries, and time periods  

---

## 📂 Dataset
The dataset used is **hotel_bookings.csv**, which includes columns such as:
- **hotel** – Type of hotel (Resort or City)  
- **is_canceled** – Reservation status (0 = Not canceled, 1 = Canceled)  
- **reservation_status_date** – Date of reservation status  
- **adr** – Average Daily Rate  
- **country** – Guest country of origin  
- **market_segment** – Type of market segment (Direct, Online TA, Corporate, etc.)  

> ⚠️ The dataset may contain missing values in some columns (e.g., `company`, `agent`) which are handled during preprocessing.  

---

## ⚙️ Steps Performed
### 1. Data Preprocessing
- Converted `reservation_status_date` to datetime format  
- Removed unnecessary columns (`company`, `agent`)  
- Handled missing values by dropping null rows  
- Ensured correct data types for categorical and numeric variables  

### 2. Exploratory Data Analysis (EDA)
- Checked shape, column names, and data types  
- Examined unique values of categorical columns  
- Created summary statistics (`describe()`)  

### 3. Data Cleaning
- Filtered out inconsistent or extreme values (`adr` < 5000)  
- Ensured cancellation column contains only binary values (0, 1)  
- Extracted month from `reservation_status_date` for trend analysis  

### 4. Visualizations
- **Reservation Status Count**: Bar chart showing canceled vs. non-canceled reservations  
- **Hotel-wise Cancellations**: Count plot comparing cancellations across Resort and City hotels  
- **ADR Trends**: Line plots showing average daily rate over time for canceled vs. non-canceled bookings  
- **Monthly Reservation Status**: Count plot of cancellations by month  
- **Top 10 Countries with Cancellations**: Pie chart visualization  
- **Market Segment Analysis**: Percentage breakdown of cancellations by market segment  

---

## 📊 Key Insights
- **High cancellation rates** are observed in both City and Resort hotels, but trends differ by hotel type.  
- **ADR (Average Daily Rate)** tends to vary significantly between canceled and non-canceled bookings.  
- **Seasonality**: Cancellations show monthly variation, indicating possible seasonal effects.  
- **Top Countries**: A few countries account for the majority of cancellations.  
- **Market Segments**: Certain booking channels (e.g., Online TA) contribute more to cancellations.  

---

## 🛠️ Tech Stack
- **Python**  
- **Pandas** – Data cleaning and preprocessing  
- **Matplotlib & Seaborn** – Data visualization  
- **Jupyter Notebook** – Interactive analysis  

---

## 🚀 How to Run
1. Clone the repository or download the project.  
2. Install required dependencies:
   ```bash
   pip install pandas matplotlib seaborn

