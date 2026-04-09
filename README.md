# 🛒 Capstone Project: E-Commerce Order Processing with DataWeave

## 📌 Project Overview

This project focuses on transforming and analyzing e-commerce order data
using MuleSoft DataWeave functional operators.

The goal is to process incoming JSON order data and generate a
structured response.

------------------------------------------------------------------------

## 🎯 Objective

Apply the following DataWeave operations:

-   map\
-   filter\
-   find\
-   groupBy\
-   mapObject\
-   filterObject

------------------------------------------------------------------------

## 📥 Input Data

The system receives order data in JSON format containing:

-   Orders (customer, country, amount, status)
-   Metadata (currency, source, generatedBy)

------------------------------------------------------------------------

## ⚙️ Tasks

### 1. Transform Orders (map)

Convert each order into: - id - customerName - totalAmount - orderStatus

------------------------------------------------------------------------

### 2. Filter High Value Orders (filter)

Return only orders where:

    amount > 100

------------------------------------------------------------------------

### 3. Find Cancelled Order (find)

Retrieve the first order where:

    status == "CANCELLED"

------------------------------------------------------------------------

### 4. Group Orders by Country (groupBy)

Example output:

``` json
{
  "Ethiopia": [...],
  "Kenya": [...],
  "USA": [...]
}
```

------------------------------------------------------------------------

### 5. Transform Metadata (mapObject)

-   Convert all keys to uppercase
-   Keep values unchanged

Example:

``` json
{
  "CURRENCY": "USD",
  "SOURCE": "OnlineStore",
  "GENERATEDBY": "OrderService"
}
```

------------------------------------------------------------------------

### 6. Filter Metadata (filterObject)

Remove:

    source

------------------------------------------------------------------------

## 📤 Final Output Structure

``` json
{
  "processedOrders": [],
  "highValueOrders": [],
  "cancelledOrder": {},
  "ordersByCountry": {},
  "metadataTransformed": {},
  "metadataFiltered": {}
}
```

------------------------------------------------------------------------

## 🛠️ Technologies Used

-   MuleSoft
-   DataWeave 2.0
-   JSON Processing

------------------------------------------------------------------------

## 📚 Reference

Based on the capstone project document provided. fileciteturn0file0

------------------------------------------------------------------------

## 🚀 Author

Capstone Project Submission
