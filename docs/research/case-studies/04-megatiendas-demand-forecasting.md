# Case Study: Megatiendas Demand Forecasting

## Source

Project:
Modelo de pronósticos de demanda para la optimización de la cadena de suministros en supermercados MEGATIENDAS

Organization:
Megatiendas

Institution:
Pontificia Universidad Javeriana Cali

Country:
Colombia

Year:
2024

Industry:
Retail / Supermarkets

Domain:
Demand Intelligence / Inventory Optimization / Supply Chain

Authors:
- Aldair de Jesús Blanco Segura
- Angie Alexandra Cantillo Martínez

Academic Program:
Master's Degree in Data Science

Primary Source:
https://vitela.javerianacali.edu.co/items/9961a5e2-b5e6-4836-80d7-2db1bbe8419c

DOI:
https://doi.org/10.71618/mj2p-zx68

---

## Business Context

Megatiendas is a Colombian supermarket chain operating multiple retail
locations.

At the time of the study, the company operated 25 stores.

Managing inventory across multiple stores creates a complex demand-planning
problem because demand varies depending on factors such as:

- Store
- Product
- Historical sales
- Promotions
- Time
- Product availability

Forecasting errors can directly affect purchasing and inventory decisions.

---

## Business Problem

Megatiendas experienced logistical problems caused by inaccurate demand
forecasts.

The main consequences included:

- Excessive purchasing
- Excess inventory
- Waste of perishable products
- Increased operating costs
- Inventory availability problems
- Inefficient supply-chain decisions

The company therefore needed a more accurate way to predict daily product
demand.

The fundamental business question was:

How much of each product will each store need?

---

## Business Objective

The project aimed to develop and implement a machine learning model capable
of predicting daily demand more accurately.

The business objective was not forecasting for its own sake.

Better forecasts were expected to support:

- Inventory planning
- Purchasing decisions
- Product availability
- Reduction of excess inventory
- Reduction of product waste
- Supply-chain optimization

---

## Data

The project used historical sales information from Megatiendas.

Important variables included:

- Store
- Product
- Historical sales
- Promotions
- Units sold
- Temporal information

The data therefore contained both historical demand behavior and contextual
variables that could influence future demand.

---

## Data Preparation

Before training predictive models, the researchers performed:

Extraction
↓
Transformation
↓
Cleaning
↓
Feature preparation
↓
Modeling

A module was developed in R to automate part of the data-management process.

This module helped extract, transform and clean historical sales information.

This is an important part of the case because the forecasting model depended
on a reliable data pipeline.

---

## Forecasting Approaches

The researchers evaluated three main forecasting approaches:

### ARMA

Autoregressive Moving Average models use historical values and previous
forecasting errors to model time-series behavior.

### SARIMAX

Seasonal AutoRegressive Integrated Moving Average with eXogenous variables
extends traditional time-series forecasting by incorporating seasonality and
external variables.

### Gradient Boosting

Gradient Boosting is a machine learning ensemble technique that combines
multiple weak predictive models to produce a stronger model.

This approach can capture nonlinear relationships between variables.

---

## Model Comparison

The three approaches were evaluated using multiple forecasting metrics.

These included:

- MAE — Mean Absolute Error
- MSE — Mean Squared Error
- RMSE — Root Mean Squared Error
- MAPE — Mean Absolute Percentage Error
- R² — Coefficient of Determination

The objective was not simply to train a model but to compare alternative
approaches and determine which produced the most useful forecasts.

---

## Results

Gradient Boosting produced the strongest overall forecasting performance
compared with ARMA and SARIMAX.

The study reports forecast accuracy above:

**85%**

for the resulting forecasting approach.

Gradient Boosting showed the strongest performance across the principal
evaluation metrics.

However, performance was not identical across every store and product.

Some store-product combinations were more difficult to forecast than others.

---

## Important Finding: Stockouts Affect Forecasting

One particularly important observation involved inventory shortages.

When a product is unavailable, recorded sales do not necessarily represent
true customer demand.

For example:

Observed Sales = 0

does not necessarily mean:

Customer Demand = 0

It could mean:

Inventory = 0
→ Product unavailable
→ Customer cannot purchase
→ Recorded sales underestimate actual demand

This distinction is important for any demand-intelligence system.

Historical sales and historical demand are not always equivalent.

---

## Business Impact

The forecasting approach supported improvements in:

- Inventory management
- Fresh-product management
- Product availability
- Purchasing decisions
- Supply-chain planning
- Strategic decision making

The research also reports reductions in excess inventory and product waste
associated with improved forecasting.

However, the study should not be interpreted as establishing a complete
long-term financial ROI for production deployment.

---

## Decision-Support Architecture

The Megatiendas case can be represented as:

Historical Sales
        ↓
Data Extraction
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Demand Forecasting
        ↓
Expected Demand
        ↓
Inventory Decision
        ↓
Purchasing / Replenishment
        ↓
Business Outcome

This is important because the forecast itself is not the final business
decision.

The forecast informs another decision.

---

## Key Findings

### 1. Existing sales data can become predictive intelligence

Megatiendas already generated the fundamental information required for the
project through normal retail operations.

The opportunity came from transforming that historical information into
future demand estimates.

---

### 2. Forecasting accuracy can vary across locations

A model that performs well for one store may perform differently for another.

Demand Intelligence therefore needs to consider differences between:

- Locations
- Products
- Customer behavior
- Inventory conditions
- Promotions

---

### 3. Promotions matter

Promotional activity can influence demand and should therefore be considered
when predicting future sales.

Historical sales alone may not capture all the factors influencing demand.

---

### 4. Sales are not always equal to demand

Stockouts can distort historical sales information.

A product cannot generate recorded sales when it is unavailable, even when
customers wanted to purchase it.

This means that a Demand Intelligence system should ideally consider both:

Sales Data
+
Inventory Availability

---

### 5. Machine learning can outperform traditional forecasting

In this particular dataset and implementation, Gradient Boosting produced
better results than the ARMA and SARIMAX alternatives evaluated.

This does not mean Gradient Boosting should automatically be selected for
other businesses.

Model selection should depend on the characteristics of each dataset.

---

### 6. Data engineering is part of the product

The researchers developed an R module for:

- Extraction
- Transformation
- Cleaning
- Data preparation

This reinforces a pattern observed in other Gintech case studies:

Machine Learning alone is not the complete solution.

---

## Limitations

### Model Generalization

Results obtained from Megatiendas cannot automatically be assumed to apply
to other retailers.

Different companies may have different:

- Product portfolios
- Store structures
- Promotion strategies
- Customer behavior
- Data quality

---

### Data Availability

Demand forecasting depends on sufficient historical information.

New products or stores may have limited historical data.

---

### Stockout Distortion

Historical sales can underestimate true demand when products were unavailable.

Inventory information may therefore be required to properly interpret sales
history.

---

### External Variables

Future versions could incorporate additional variables such as:

- Holidays
- Weather
- Local events
- Economic conditions
- Competitor activity
- Pricing
- Promotional intensity

These variables could potentially improve forecasting performance.

---

## Gintech Relevance

This case is highly relevant to the Demand Intelligence opportunity.

Unlike a global enterprise case, Megatiendas demonstrates that demand
forecasting can be applied within a Colombian retail environment using
business data already generated by normal operations.

A potential Gintech workflow could be:

POS / ERP
    ↓
Historical Sales
    ↓
Inventory
    ↓
Promotions
    ↓
Data Quality
    ↓
Demand Forecast
    ↓
Business Recommendation
    ↓
Inventory / Purchasing Decision

---

## Potential Gintech Opportunity

Gintech should not necessarily position the product as:

"AI Demand Forecasting"

because forecasting alone does not solve the business problem.

A stronger product concept could be:

Demand Intelligence
        ↓
Expected Demand
        ↓
Inventory Risk
        ↓
Recommended Action

For example:

Expected high demand
+
Low inventory
        ↓
Stockout Risk
        ↓
Increase replenishment

or:

Expected low demand
+
High inventory
        ↓
Overstock Risk
        ↓
Reduce purchasing / consider promotion

The prediction becomes valuable when translated into an operational decision.

---

## Potential Product Inputs

A first Demand Intelligence product could potentially use:

- Historical sales
- Current inventory
- Product
- Store/location
- Promotions
- Price
- Calendar information

More advanced versions could incorporate:

- Weather
- Holidays
- Local events
- Economic indicators
- Supplier lead times

---

## Potential Product Outputs

Instead of only displaying a demand forecast, Gintech could potentially
generate:

- Expected demand
- Stockout risk
- Overstock risk
- Inventory recommendations
- Purchasing recommendations
- Product prioritization
- Location-level alerts
- Forecast confidence

---

## Example Decision

Traditional Dashboard:

Product A
Forecast: 420 units

Potential Gintech Decision Intelligence:

Product A
Expected demand: 420 units
Current inventory: 270 units
Expected shortage: 150 units
Stockout risk: High

Recommended Action:
Increase replenishment before the next demand period.

The second output is closer to a business decision than a standalone
forecast.

---

## Comparison With Nestlé

Nestlé:

Historical Demand
+
Product Relationships
+
Business Information
        ↓
Demand Forecast
        ↓
Demand Planning

Megatiendas:

Historical Sales
+
Store
+
Product
+
Promotions
        ↓
Daily Demand Forecast
        ↓
Inventory Planning

Both cases support Demand Intelligence.

However, Megatiendas provides regional evidence that the problem also exists
within Colombian retail operations.

---

## Pattern Across Regional Cases

AI4Time:

SAP Maintenance Data
        ↓
Prediction
        ↓
Maintenance Decision

Megatiendas:

Retail Sales Data
        ↓
Prediction
        ↓
Inventory Decision

This suggests a broader product pattern:

Existing Business Data
        ↓
Understand
        ↓
Predict
        ↓
Assess Risk
        ↓
Recommend
        ↓
Business Decision

The industry and data change.

The decision-intelligence pattern remains similar.

---

## Product Hypothesis

Can Gintech use historical sales, inventory and operational data that
retailers already generate to predict future demand, identify inventory
risks and recommend purchasing or replenishment actions?

---

## Potential Gintech Capability

Primary:

Demand Intelligence

Supporting Capabilities:

- Data Integration
- Data Quality
- Demand Forecasting
- Inventory Analytics
- Machine Learning
- Business Intelligence
- Decision Support

---

## Research Classification

Region:
Colombia / Latin America

Industry:
Retail / Supermarkets

Primary Opportunity:
Demand Intelligence

Secondary Opportunity:
Operations Intelligence

Research Phase:
Regional Validation

---

## Evidence Strength

Primary source available:
Yes

Full document available:
Yes

Real organization:
Yes

Real operational data:
Yes

Multiple models compared:
Yes

Business application:
Yes

Long-term production ROI demonstrated:
No

---

## Key Product Principle

Do not stop at predicting what will happen.

Translate the prediction into the business decision that should happen next.

---

## Status

Research completed
