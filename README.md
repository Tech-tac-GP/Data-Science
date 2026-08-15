# Tech-tac — Data Science

## Project Overview

**Tech-tac** is an e-commerce platform specialized in electronics.

This project focuses on analyzing customer behavior and e-commerce activity to understand **customer interactions, product performance, category and brand demand, purchasing patterns, time-based activity, and the customer journey from viewing a product to purchasing it.**

---

## Dataset

The dataset contains customer events from an electronics e-commerce store.

Each row represents an event performed by a customer.

### Event Types

* **View** - Customer viewed a product
* **Cart** - Customer added a product to the cart
* **Purchase** - Customer purchased a product

### Main Features

| Column          | Description                 |
| --------------- | --------------------------- |
| `event_time`    | Date and time of the event  |
| `event_type`    | Type of customer event      |
| `product_id`    | Product identifier          |
| `category_id`   | Category identifier         |
| `category_code` | Product category            |
| `brand`         | Product brand               |
| `price`         | Product price               |
| `user_id`       | Customer identifier         |
| `user_session`  | Customer session identifier |

---

## 🧹 Data Cleaning & Preparation

The dataset was prepared before performing the exploratory analysis.

The main steps included:

* Checking the dataset structure and data types
* Handling missing values
* Checking duplicated and inconsistent data
* Analyzing price outliers
* Extracting date and hour from `event_time`
* Splitting `category_code` into category levels
* Checking user and session consistency
* Saving the cleaned dataset for further analysis

---

## Exploratory Data Analysis

The analysis covered several aspects of the e-commerce activity.

### 1. Customer Funnel

The customer journey was analyzed through:

**View → Cart → Purchase**

Conversion rates:

* **View → Cart:** 6.81%
* **Cart → Purchase:** 69.12%
* **View → Purchase:** 4.71%

This helps identify how customers move through the purchasing process and where the largest drop-off occurs.

### 2. Product Analysis

Products were analyzed based on:

* Views
* Cart additions
* Purchases

This identifies products receiving high customer interest and products generating purchases.

### 3. Category Analysis

Categories were analyzed across views, cart additions, and purchases to identify the product categories with the highest customer demand.

### 4. Brand Analysis

Brands were compared based on customer interactions and purchases to identify the most active and popular brands.

### 5. Time Analysis

Customer activity was analyzed by:

* Date
* Hour

This helps identify periods with higher levels of customer activity.

### 6. Price Analysis

Price analysis included:

* Price distribution
* Price statistics
* Average price by category

The analysis also examined price outliers and differences in average prices across categories.

---

## Visualizations

The main visualizations created during the analysis are available in the `outputs/` folder.

They include:

* Customer Funnel
* Top Products
* Top Categories
* Top Brands
* Customer Activity by Date
* Customer Activity by Hour
* Price Distribution
* Average Price by Category

---

## Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook**

---

## Project Structure

```text
Data-Science/
│
├── data/
│   ├── events.csv
│   └── cleaned_events.csv
│
├── notebooks/
│   └── data_science.ipynb
│
├── outputs/
│   └── Visualizations
│
└── README.md
```

---

## Key Findings

* The majority of customer events are **product views**, while only a smaller percentage result in cart additions and purchases.
* The **View → Cart conversion rate is 6.81%**, showing a significant drop between viewing and adding products to the cart.
* The **Cart → Purchase conversion rate is 69.12%**, indicating that customers who add products to their carts are relatively likely to complete a purchase.
* A small number of products and categories receive a large share of customer interactions.
* Customer activity varies throughout the day, with noticeable differences between active and less active hours.
* Product prices are highly skewed, with a small number of very expensive products affecting the overall average price.

---

## Project Team

**Tech-tac-GP — Data Science Team**
