# 🏨 Hotel Booking Data Analysis & EDA

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a hotel booking dataset to identify important patterns and insights related to hotel bookings, cancellations, customer types, booking channels, room types, and other factors.

The analysis helps understand **customer booking behavior and cancellation patterns** using Python and data visualization techniques.

---

## 🎯 Objectives

The main objectives of this project are:

* Analyze hotel booking data using Exploratory Data Analysis.
* Understand booking and cancellation patterns.
* Compare **City Hotel** and **Resort Hotel** bookings.
* Analyze customer types and booking channels.
* Identify factors associated with booking cancellations.
* Handle missing and inconsistent data.
* Create meaningful visualizations.
* Generate useful insights from the dataset.

---

## 📊 Dataset

The dataset contains information about hotel reservations, including:

* Hotel type
* Booking status
* Lead time
* Arrival date
* Number of guests
* Number of stays
* Number of adults, children and babies
* Meal type
* Country
* Market segment
* Distribution channel
* Is repeated guest
* Previous bookings
* Reserved and assigned room types
* Booking changes
* Deposit type
* Customer type
* ADR (Average Daily Rate)
* Reservation status

### Dataset Summary

| Attribute              |  Value |
| ---------------------- | -----: |
| Total Rows             | 87,396 |
| Total Columns          |     33 |
| City Hotel Bookings    | 53,428 |
| Resort Hotel Bookings  | 33,968 |
| Non-Cancelled Bookings | 63,371 |
| Cancelled Bookings     | 24,025 |
| Cancellation Rate      | 27.49% |

---

## 🛠️ Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**

---

## 🔍 Project Workflow

### 1. Data Loading

The hotel booking dataset is loaded into a Pandas DataFrame.

### 2. Data Cleaning

* Checked missing values.
* Handled missing values.
* Removed unnecessary/inconsistent data where required.
* Checked duplicate records.
* Verified data types.

### 3. Exploratory Data Analysis

Different aspects of the dataset were analyzed, including:

* Hotel type distribution
* Cancellation status
* Customer type
* Market segment
* Distribution channel
* Room type
* Booking lead time
* Average Daily Rate
* Repeated guests
* Arrival patterns

### 4. Data Visualization

Different charts were created to understand patterns in the data, such as:

* Bar charts
* Count plots
* Histograms
* Pie charts
* Box plots
* Correlation heatmaps

---

## 📈 Key Findings

Some important observations from the analysis include:

* **City Hotel** has more bookings than Resort Hotel.
* Approximately **27.49% of bookings were cancelled**.
* The dataset contains substantially more non-cancelled bookings than cancelled bookings.
* Customer type and market segment provide useful information about booking behavior.
* Lead time and other booking-related variables can be analyzed to understand cancellation patterns.
* Different hotel types show differences in customer and booking characteristics.

---

## 📂 Project Structure

```text
hotel-booking-eda/
│
├── data/
│   └── hotel_bookings.csv
│
├── notebooks/
│   └── Hotel_Booking_EDA.ipynb
│
├── report/
│   └── Hotel_Booking_EDA_Report.pdf
│
├── images/
│   ├── hotel_distribution.png
│   ├── cancellation_analysis.png
│   ├── customer_type.png
│   └── correlation_heatmap.png
│
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run the Project

### Using Google Colab

1. Download or clone this repository.
2. Open `Hotel_Booking_EDA.ipynb`.
3. Upload the dataset.
4. Run the notebook cells sequentially.

### Required Libraries

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 📌 Project Type
