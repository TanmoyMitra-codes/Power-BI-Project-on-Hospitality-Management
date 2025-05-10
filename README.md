
# 📊 Hotel Booking Analysis Dashboard

This repository contains datasets and documentation for a Power BI dashboard focused on analyzing hotel booking data. The dashboard visualizes trends in bookings, platform usage, revenue, room capacity, and customer ratings.

🔗 **Dashboard Link**: [Power BI Report](https://app.powerbi.com/view?r=eyJrIjoiZjM0MjUxYWYtNzQ1NC00OTgzLTk5Y2UtNWFiMDU3YjMxOTUxIiwidCI6IjQwN2U0NzE2LTFkNjgtNGIxOS04Yjc4LWE4YWQwNzQ3ZWNjOSIsImMiOjEwfQ%3D%3D)

---

## 📁 Datasets

### 1. `fact_bookings.csv`
Detailed individual booking records.

| Column              | Description                                      |
|---------------------|--------------------------------------------------|
| booking_id          | Unique booking reference                         |
| property_id         | Identifier of the hotel property                 |
| booking_date        | Date when the booking was made                   |
| check_in_date       | Scheduled check-in date                          |
| checkout_date       | Scheduled checkout date                          |
| no_guests           | Number of guests per booking                     |
| room_category       | Category/type of room booked                     |
| booking_platform    | Booking source (e.g., direct, logtrip, others)   |
| ratings_given       | Guest-provided rating                            |
| booking_status      | Status of the booking (e.g., Cancelled, Checked Out) |
| revenue_generated   | Revenue expected                                 |
| revenue_realized    | Revenue after adjustments                        |

### 2. `fact_aggregated_bookings.csv`
Aggregated daily room data by property and category.

| Column               | Description                         |
|----------------------|-------------------------------------|
| property_id          | Hotel property ID                   |
| check_in_date        | Booking check-in date               |
| room_category        | Room type                           |
| successful_bookings  | Number of completed bookings        |
| capacity             | Total capacity for that room type   |

### 3. `dim_date.csv`
Date dimension table for time-based filtering and grouping.

| Column    | Description                  |
|-----------|------------------------------|
| date      | Calendar date                |
| mmm yy    | Month and year format        |
| week no   | Week number in the year      |
| day_type  | Type of day (weekday/weekend)|

---

## 📈 Dashboard Features

The Power BI dashboard provides a comprehensive overview of hotel performance metrics, offering valuable insights into guest behavior, revenue, and distribution channels.

### 1. Booking Trends Over Time
- **Monthly Guest Counts by Country**: See how many guests visit from different countries each month.
- **Average Length of Stay**: Analyze how long guests stay on average.
- **Cancellations and Bookings per Month**: Understand monthly trends in cancellations and bookings.

### 2. Revenue Analysis
- **Revenue Gains and Losses**: Monitor revenue changes over time.
- **Revenue by Distribution Channel**: Identify the most profitable booking platforms.

### 3. Occupancy and Capacity
- **Room Occupancy Rates**: Measure how well different room categories are utilized.
- **Capacity Utilization**: Assess if room capacities are being fully used.

### 4. Booking Platform Performance
- **Platform Comparison**: Compare performance across platforms like Direct and Logtrip.

### 5. Customer Feedback
- **Guest Ratings**: Track customer satisfaction through ratings.

---

## 🛠️ Usage Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/hotel-booking-dashboard.git
   ```

2. **Access the Dashboard**:
   - Open the Power BI `.pbix` file (if available) or view it online.

3. **Explore the Data**:
   - Use the datasets for deeper insights or transformation tasks.

---

## 📌 Notes

- Ratings may be missing for some bookings.
- Ensure dates are in a consistent format (`YYYY-MM-DD` or `DD-MMM-YY`).
- Use `booking_status` to exclude cancelled bookings for clean revenue analysis.

---

## 📧 Contact

For questions or collaboration, reach out via GitHub issues.
