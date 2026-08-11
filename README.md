# 🚕 Ola Booking Analysis

## 1. Project Title

### 🚕 Ola Booking Analysis: Ride Performance & Business Insights Dashboard

An interactive Power BI dashboard designed to analyze Ola booking performance,
vehicle-wise demand, revenue, cancellations, ride distance, and customer and
driver ratings.

## 2. Short Description

The Ola Booking Analysis Dashboard is an interactive business intelligence
project developed to analyze 103K+ ride-booking records from Bengaluru over a
one-month period.

The project focuses on understanding overall booking performance, successful
and cancelled rides, vehicle-wise ride demand and distance, revenue
contribution by payment method, high-value customers, cancellation patterns,
and customer and driver satisfaction.

The analysis combines Excel, SQL, Power Query, Power BI, and DAX to transform
raw booking data into a five-page interactive dashboard.

The dashboard helps identify operational bottlenecks, vehicle performance
patterns, revenue opportunities, cancellation issues, and customer experience
trends to support data-driven business decisions.

## 3. Tech Stack

### Technologies & Tools

The project was developed using the following tools and technologies:

- **Microsoft Excel** – Used for initial data inspection, data cleaning,
  validation, formatting, and preparation.
- **SQL / PostgreSQL** – Used for data exploration, filtering, aggregation,
  business analysis, and answering key analytical questions.
- **Power Query** – Used for data transformation and preparation within
  Power BI.
- **Power BI Desktop** – Used to create the interactive five-page dashboard
  and business visualizations.
- **DAX (Data Analysis Expressions)** – Used to create calculated measures,
  KPIs, booking metrics, cancellation analysis, revenue analysis, and
  rating-related calculations.
- **Data Visualization** – Used KPI cards, bar charts, line charts, donut
  charts, tables, scatter plots, and other visuals to communicate insights.
- **Git & GitHub** – Used for project version control, documentation, and
  portfolio presentation.
- **File Formats** – `.pbix` for the Power BI dashboard, `.csv` for the
  dataset, `.sql` for SQL analysis, and `.png` for dashboard previews.

## 4. Data Source

###  Source: Ola Booking Project Dataset

The dataset is a project-based ride-booking dataset created for a Bengaluru
city ride-booking analysis scenario covering one month of booking activity.

The uploaded dataset contains **103,024 booking records** and includes
information related to booking status, customers, vehicle types, locations,
waiting/arrival times, cancellations, incomplete rides, booking value,
payment methods, ride distance, and customer and driver ratings.

### Key Data Fields

The dataset includes:

- Date
- Time
- Booking ID
- Booking Status
- Customer ID
- Vehicle Type
- Pickup Location
- Drop Location
- V.TAT
- C.TAT
- Customer Cancellation Reason
- Driver Cancellation Reason
- Incomplete Rides
- Incomplete Ride Reason
- Booking Value
- Payment Method
- Ride Distance
- Driver Rating
- Customer Rating

### Data Preparation

The data analysis workflow included:

1. Initial data inspection in Excel.
2. Data cleaning and validation.
3. SQL-based data exploration and business analysis.
4. Power Query transformation.
5. Power BI data modeling.
6. DAX measure creation.
7. Interactive dashboard development.
8. Business insight generation.

# 5. Features / Highlights

##  Business Problem

A ride-booking platform generates large amounts of operational data across
bookings, vehicles, customers, cancellations, revenue, ride distance, and
ratings.

However, raw booking data makes it difficult for business stakeholders to
quickly understand:

- How many bookings are successfully completed.
- Where bookings are being lost through cancellations or driver availability.
- Which vehicle types contribute the most ride distance.
- Which payment methods generate the most booking value.
- Which customers contribute the highest booking value.
- Why customers and drivers cancel rides.
- How customer and driver satisfaction varies across rides.
- Where operational improvements can increase booking completion and
  customer satisfaction.

Without a centralized analytical solution, it becomes difficult to identify
operational bottlenecks, optimize vehicle utilization, reduce cancellations,
and make data-driven decisions.

The project therefore transforms raw Ola booking data into an interactive
business intelligence dashboard for monitoring booking performance, vehicle
performance, revenue, cancellations, and customer experience.

##  Goal of the Dashboard

The goal of the dashboard is to provide an interactive analytical solution
that helps stakeholders understand ride-booking performance from multiple
business perspectives.

The dashboard enables decision-makers to:

- Monitor overall booking volume and booking status.
- Analyze successful, cancelled, and unavailable-driver bookings.
- Compare vehicle types based on ride distance and customer ratings.
- Analyze revenue contribution by payment method.
- Identify high-value customers.
- Understand customer and driver cancellation reasons.
- Analyze incomplete ride patterns.
- Monitor customer and driver ratings.
- Identify operational bottlenecks.
- Support data-driven decisions related to ride operations, revenue, and
  customer experience.



#  Key Business Questions & Answers

The dashboard was designed around five important business questions.

## 1. What is the overall booking performance and where are bookings being lost?

The dataset contains **103,024 bookings**.

The booking-status distribution is:

| Booking Status | Bookings | Percentage |
|---|---:|---:|
| **Success** | **63,967** | **62.09%** |
| Canceled by Driver | 18,434 | 17.89% |
| Canceled by Customer | 10,499 | 10.19% |
| Driver Not Found | 10,124 | 9.83% |
| **Total** | **103,024** | **100%** |

### Business Answer

**62.09% of bookings were successfully completed**, while **37.91% did not
result in a successful ride** due to driver cancellations, customer
cancellations, or driver availability issues.

The largest non-success category is **Canceled by Driver at 17.89%**,
followed by **Canceled by Customer at 10.19%** and **Driver Not Found at
9.83%**.

### Key takeaway

> The major opportunity is to improve booking completion by reducing driver
> cancellations and addressing driver availability issues.

## 2. Which vehicle types contribute the most to ride demand and distance?

**Prime Sedan** contributes the highest total ride distance in the dataset.

| Vehicle Type | Total Ride Distance |
|---|---:|
| **Prime Sedan** | **234,535** |
| eBike | 230,842 |
| Bike | 227,746 |
| Prime Plus | 227,186 |
| Mini | 225,703 |
| Prime SUV | 223,848 |
| Auto | 92,043 |

Prime Sedan also has the highest average ride distance at approximately
**15.76 km per booking** among all vehicle types.

### Business Answer

> **Prime Sedan is the strongest vehicle type by total ride distance, covering
> approximately 234,535 km.** eBike and Bike also contribute substantial ride
> distance, while Auto has significantly lower average and total distance.

### Key takeaway

> Premium car categories such as Prime Sedan demonstrate strong utilization
> by ride distance, while Auto is more concentrated in shorter-distance trips.

## 3. Which payment methods and customers contribute most to booking revenue?

The dataset generated approximately **₹35.08 million** in booking value from
successful rides.

Revenue by payment method:

| Payment Method | Successful Bookings | Booking Value |
|---|---:|---:|
| **Cash** | **35,022** | **₹19.26M** |
| **UPI** | **25,881** | **₹14.17M** |
| Credit Card | 2,435 | ₹1.31M |
| Debit Card | 629 | ₹0.34M |
| **Total** | **63,967** | **₹35.08M** |

### Business Answer

> **Cash is the largest revenue-contributing payment method, generating
> approximately ₹19.26M, followed by UPI at approximately ₹14.17M.**
> Together, these two payment methods account for the majority of successful
> booking value.

The dashboard also identifies the **Top 5 Customers by Total Booking Value**,
helping the business identify high-value customers for potential retention
and loyalty strategies.

### Key takeaway

> Cash and UPI dominate booking-value contribution, while high-value customer
> analysis provides an opportunity for targeted retention and loyalty
> initiatives.

## 4. What are the major reasons for customer and driver cancellations?

###  Customer Cancellation Reasons

The most common customer cancellation reasons are:

| Customer Cancellation Reason | Cancellations |
|---|---:|
| **Driver is not moving towards pickup location** | **3,175** |
| Driver asked to cancel | 2,670 |
| Change of plans | 2,081 |
| AC is Not working | 1,568 |
| Wrong Address | 1,005 |

###  Driver Cancellation Reasons

The most common driver cancellation reasons are:

| Driver Cancellation Reason | Cancellations |
|---|---:|
| **Personal & Car related issue** | **6,542** |
| Customer related issue | 5,413 |
| Customer was coughing/sick | 3,654 |
| More than permitted people in the vehicle | 2,825 |

### Business Answer

> **Driver-side operational issues are the largest cancellation concern.**
> Personal and car-related issues account for 6,542 driver cancellations,
> while the most common customer-side reason is that the driver was not
> moving toward the pickup location, accounting for 3,175 cancellations.

### Key takeaway

> Reducing driver-related operational issues and improving driver movement
> toward pickup locations could have a meaningful impact on booking
> completion and customer experience.

## 5. How does customer and driver satisfaction vary across the ride network?

Overall ratings are very stable:

- **Average Driver Rating: approximately 4.00**
- **Average Customer Rating: approximately 4.00**

The relationship between customer and driver ratings is approximately **0.00
correlation**, indicating almost no linear relationship between the two
ratings in this dataset.

### Average Customer Rating by Vehicle Type

| Vehicle Type | Avg. Customer Rating |
|---|---:|
| **Prime Plus** | **4.01** |
| Prime Sedan | 4.00 |
| Prime SUV | 4.00 |
| Auto | 4.00 |
| Mini | 4.00 |
| Bike | 3.99 |
| eBike | 3.99 |

### Business Answer

> Customer and driver ratings remain consistently close to **4.00 across the
> dataset**, with only minor differences between vehicle types. Prime Plus
> records the highest average customer rating at approximately **4.01**,
> while eBike has the lowest at approximately **3.99**.

### Key takeaway

> Overall customer satisfaction is stable across vehicle categories, but
> rating analysis can still be used to monitor small differences in service
> quality and identify areas for continuous improvement.

#  Walkthrough of Key Visuals

## 1.  Overall Performance

The **Overall** page provides a high-level view of booking activity and
operational performance.

###  Ride Volume Over Time

A time-series chart displays the number of bookings across the month.

**Purpose:**

> Helps stakeholders monitor changes in booking demand and identify periods
> with higher or lower ride activity.

###  Booking Status Breakdown

A booking-status visual compares:

- Successful bookings
- Canceled by Customer
- Canceled by Driver
- Driver Not Found

**Purpose:**

> Provides an immediate overview of successful rides and the major sources
> of booking loss.

### Business Insight

> With a **62.09% successful booking rate**, more than one-third of booking
> attempts do not result in successful rides, creating an important
> operational improvement opportunity.



# 2.  Vehicle Type Analysis

The **Vehicle Type** page focuses on vehicle utilization and customer
experience.

###  Top Vehicle Types by Ride Distance

Ranks vehicle types according to total ride distance.

**Key finding:**

> Prime Sedan ranks first with approximately **234,535 km** of total ride
> distance.

###  Average Customer Rating by Vehicle Type

Compares customer satisfaction across vehicle categories.

**Key finding:**

> Prime Plus records the highest average customer rating at approximately
> **4.01**, while rating differences across vehicle types are relatively
> small.

### Business Purpose

> Helps operations teams understand which vehicle types have stronger
> utilization and how customer satisfaction varies by vehicle category.

# 3.  Revenue Analysis

The **Revenue** page focuses on booking value, payment behavior, customers,
and ride distance.

###  Revenue by Payment Method

Compares booking value generated through different payment methods.

**Key finding:**

> Cash contributes approximately **₹19.26M**, followed by UPI at
> approximately **₹14.17M**.

###  Top 5 Customers

Identifies customers contributing the highest total booking value.

**Business purpose:**

> Helps identify high-value customers who may be important for retention,
> loyalty programs, and targeted customer engagement.

###  Ride Distance Distribution

Shows how ride distances are distributed across the booking data.

**Business purpose:**

> Helps understand short- and long-distance ride patterns and provides
> additional context for vehicle utilization and booking value.

# 4.  Cancellation Analysis

The **Cancellation** page focuses on identifying why bookings are lost.

###  Customer Cancellation Reasons

Highlights the most common reasons customers cancel rides.

**Key finding:**

> The most common customer cancellation reason is **"Driver is not moving
> towards pickup location"**, with **3,175 cancellations**.

###  Driver Cancellation Reasons

Highlights the reasons drivers cancel rides.

**Key finding:**

> **Personal & Car related issue** is the largest driver cancellation reason,
> with **6,542 cancellations**.

### Business Purpose

> Identifying the root causes of cancellations helps the business focus
> operational improvements on the highest-impact problems.

---

# 5.  Ratings Analysis

The **Ratings** page evaluates customer and driver experience.

###  Driver Rating Distribution

Shows how driver ratings are distributed across the booking dataset and
vehicle categories.

###  Customer Rating Distribution

Shows the distribution of customer ratings for successful rides.

###  Customer vs Driver Ratings

Compares customer and driver ratings for completed rides.

**Key finding:**

> Both average ratings are approximately **4.00**, while their correlation is
> close to zero, indicating little linear relationship between customer and
> driver ratings.

### Business Purpose

> Rating analysis helps monitor service quality, identify rating patterns,
> and support continuous customer-experience improvements.

#  Key Insights

## 1.  Booking Success Is the Major Operational KPI

Only **62.09% of the 103,024 bookings** were successful.

The remaining bookings were lost through:

- Driver cancellations
- Customer cancellations
- Driver Not Found

**Insight:**

> Improving booking completion should be a major operational priority because
> every unsuccessful booking represents a potential lost ride and revenue
> opportunity.

## 2.  Prime Sedan Has the Highest Ride-Distance Contribution

Prime Sedan records approximately **234,535 km**, the highest total ride
distance among vehicle types.

**Insight:**

> Prime Sedan demonstrates strong utilization and may represent an important
> vehicle category for maintaining ride availability and operational capacity.

## 3.  Cash and UPI Dominate Revenue Contribution

Cash contributes approximately **₹19.26M**, while UPI contributes approximately
**₹14.17M** in successful booking value.

**Insight:**

> Cash and UPI are the dominant payment channels and should remain important
> components of the platform's payment strategy.

## 4.  Driver-Related Issues Are a Major Cancellation Problem

Driver cancellations account for **17.89%** of all bookings.

The largest driver cancellation reason is:

> **Personal & Car related issue — 6,542 cancellations**

**Insight:**

> Operational and vehicle-related driver issues represent a significant
> opportunity for reducing booking losses.

## 5.  Pickup-Related Issues Drive Customer Cancellations

The largest customer cancellation reason is:

> **Driver is not moving towards pickup location — 3,175 cancellations**

**Insight:**

> Improving driver movement, pickup coordination, and driver availability
> could reduce customer frustration and cancellation rates.

## 6.  Customer Satisfaction Is Relatively Stable

Average customer and driver ratings are both approximately **4.00**.

Differences across vehicle types are very small.

**Insight:**

> Overall service satisfaction is stable, but cancellation issues appear to
> be a more significant operational concern than rating performance.

#  Business Impact

## 1.  Improve Booking Completion

The dashboard identifies the percentage of successful, cancelled, and
unfulfilled bookings.

**Business Impact:**

> Reducing cancellations and driver-unavailability issues can increase the
> number of completed rides and improve revenue realization.

## 2.  Reduce Driver Cancellations

Driver cancellations represent **17.89% of all bookings**, with
personal/car-related issues being the largest driver cancellation reason.

**Business Impact:**

> Addressing vehicle reliability, driver readiness, and operational issues
> can reduce cancellations and improve booking fulfillment.

## 3.  Improve Pickup Experience

The largest customer cancellation reason is the driver not moving toward the
pickup location.

**Business Impact:**

> Improving driver tracking, pickup coordination, and driver response can
> reduce customer cancellations and improve customer experience.

## 4.  Optimize Vehicle Utilization

Prime Sedan contributes the highest total ride distance.

**Business Impact:**

> Vehicle-wise distance analysis can help operations teams better understand
> demand and optimize vehicle allocation and availability.

## 5.  Strengthen Revenue Strategy

Cash and UPI contribute the majority of successful booking value.

**Business Impact:**

> Understanding payment behavior can support payment-channel optimization and
> provide insights for digital-payment adoption initiatives.

## 6.  Retain High-Value Customers

The Top 5 Customers visual identifies customers contributing the highest
booking value.

**Business Impact:**

> High-value customers can be targeted through loyalty programs, personalized
> offers, and retention strategies.

## 7.  Maintain Service Quality

Average customer and driver ratings are approximately 4.00.

**Business Impact:**

> Continued monitoring of ratings can help maintain service quality while
> cancellation analysis focuses attention on the more significant operational
> problems.

# Screenshots

### 1.  Overall Performance

![Ola Overall Performance](./ola%201.png)

### 2.  Vehicle Type Analysis

![Ola Vehicle Type Analysis](./ola%202.png)

### 3.  Revenue Analysis

![Ola Revenue Analysis](./ola%203.png)

### 4.  Cancellation Analysis

![Ola Cancellation Analysis](./ola%204.png)

### 5.  Ratings Analysis

![Ola Ratings Analysis](./ola%205.png)

