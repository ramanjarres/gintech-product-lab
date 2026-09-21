# Case Study: Héctor Ocaña Izquierdo Logistics Planning Optimization

## Source

Project:
Sistema inteligente basado en machine learning para apoyar la optimización
de la planificación logística en la empresa Héctor Ocaña Izquierdo

Organization:
Héctor Ocaña Izquierdo

Institution:
Universidad Católica Santo Toribio de Mogrovejo (USAT)

Country:
Peru

Location:
Chiclayo

Year:
2026

Industry:
Logistics / Transportation / Distribution

Domain:
Operations Intelligence / Logistics Optimization / Demand Forecasting

Author:
Christian Paul Bellasmil Farroñan

Advisor:
Guadalupe Teresa Lip Curo

Academic Program:
Systems and Computer Engineering

Primary Source:
https://repositorio.usat.edu.pe/items/ec7594c2-5980-434f-83ee-41af795ce2c1

Persistent Identifier:
https://hdl.handle.net/20.500.12423/10182

---

## Business Context

Logistics planning requires organizations to coordinate multiple operational
decisions.

These can include:

- Expected demand
- Resource availability
- Vehicle allocation
- Delivery planning
- Route selection
- Driving time
- Distance traveled

When these decisions are performed using fragmented information or manual
planning, organizations may experience inefficient resource allocation,
longer routes and higher operational costs.

The project studied how machine learning and route optimization could support
logistics planning at the company Héctor Ocaña Izquierdo.

---

## Business Problem

The organization needed to improve its logistics planning process.

The fundamental challenge involved coordinating two connected decisions:

1. How much future demand should the company expect?
2. How should available logistics resources be deployed to serve that demand?

These decisions are interdependent.

Poor demand estimates can produce poor resource planning.

Poor route planning can increase:

- Distance traveled
- Driving time
- Resource utilization
- Operational costs
- Delivery inefficiency

The project therefore approached logistics planning as an integrated
decision problem rather than an isolated prediction task.

---

## Business Objective

The project aimed to develop an intelligent system based on machine learning
to support logistics planning.

The solution combined two principal analytical components:

1. Demand forecasting
2. Logistics route optimization

These components were integrated into a web platform designed to support
real-time logistics management.

---

## Solution Architecture

The solution can be represented conceptually as:

Historical Operational Data
        ↓
Demand Forecasting
        ↓
Expected Future Demand
        ↓
Resource Planning
        ↓
Route Optimization
        ↓
Recommended Logistics Plan
        ↓
Operational Execution

This architecture is particularly important because prediction and
optimization operate together.

---

## Model 1 — Demand Forecasting

The first model focused on predicting future demand.

The project used:

**LSTM — Long Short-Term Memory**

LSTM is a recurrent neural-network architecture designed to learn temporal
patterns and dependencies.

Conceptually:

Historical Demand
        ↓
Temporal Patterns
        ↓
LSTM
        ↓
Future Demand
        ↓
Resource Requirements

The model achieved a reported:

**93.83% precision**

according to the thesis.

This metric should be interpreted using the definition and evaluation
methodology used by the author and should not automatically be translated
into equivalent business performance.

---

## Model 2 — Route Optimization

The second analytical component focused on logistics route optimization.

Its purpose was to improve how transportation resources were used after
future logistics requirements had been estimated.

Conceptually:

Expected Demand
        ↓
Available Resources
        ↓
Logistics Constraints
        ↓
Route Optimization
        ↓
Recommended Route
        ↓
Delivery Execution

The project reports:

**99.08% precision**

for the route optimization component.

As with the demand model, this is the technical performance metric reported
by the study and should not be interpreted as a 99.08% reduction in logistics
cost or distance.

---

## Integrated Intelligence

One of the strongest characteristics of the project is that the two models
were not treated as independent experiments.

They were integrated.

Demand Forecast
        ↓
Resource Requirements
        ↓
Route Optimization
        ↓
Operational Plan

This creates a progression from:

Prediction

to:

Decision Support

The organization does not only learn what may happen.

It receives information that can influence what should be done.

---

## Web Platform

The models were integrated into a web platform.

The platform supported:

- Interaction with the analytical system
- Logistics management
- Operational planning
- Real-time interaction with the solution

This means the project went beyond developing isolated machine-learning
models.

The models became components of an operational system.

---

## Reported Results

The study reports several technical and operational results.

### Demand Forecasting

Reported precision:

**93.83%**

### Route Optimization

Reported precision:

**99.08%**

### Driving Time

Reported improvement:

**24.5%**

### Distance Traveled

Reported reduction:

**34.47%**

### System Reliability

Reported reliability under continuous operating conditions:

**99.44%**

### Defect Rate

Reported defect rate per execution:

**0.08**

### User Satisfaction

Reported user satisfaction:

**93.68%**

These results represent different dimensions of system performance and
should not be interpreted as equivalent metrics.

---

## Why Operational Metrics Matter More

The most useful results from a business perspective are not necessarily the
machine-learning metrics.

For example:

93.83% model precision

is a technical result.

But:

24.5% improvement in driving time

and:

34.47% reduction in distance traveled

are much closer to measurable operational outcomes.

This distinction is important for Gintech.

A successful Operations Intelligence product should ultimately demonstrate
improvement in business operations, not only model performance.

---

## Decision Point

The case contains a clear operational decision point:

**How should logistics resources be planned and routed to satisfy expected
demand efficiently?**

This can be decomposed into:

What demand should we expect?
        ↓
What resources will we need?
        ↓
How should those resources be allocated?
        ↓
What routes should they follow?

This is a stronger business problem than simply:

"Can we predict demand?"

---

## Key Findings

### 1. Prediction can feed optimization

Demand forecasting becomes significantly more valuable when its output is
used by another decision system.

Instead of:

Demand Forecast
→ Dashboard

the architecture becomes:

Demand Forecast
→ Resource Planning
→ Route Optimization
→ Operational Action

---

### 2. Multiple models can form one business workflow

The solution demonstrates that an intelligent business system does not need
to rely on a single model.

Different analytical components can solve different parts of the same
decision process.

---

### 3. Operational value can be measured directly

Driving time and distance traveled are operational KPIs.

This makes it possible to compare:

Before Optimization

versus:

After Optimization

This is particularly valuable when demonstrating ROI.

---

### 4. Machine learning is not necessarily the final decision engine

Machine learning predicts future demand.

Another analytical component determines how resources should respond.

This distinction is important:

Prediction answers:

"What is likely to happen?"

Optimization answers:

"What should we do about it?"

---

### 5. The interface is not the intelligence

The web platform provides access to the system.

However, the value comes from the analytical pipeline behind it.

Data
+
Prediction
+
Optimization
+
Business Rules
+
Operational Workflow

create the intelligence.

---

### 6. User adoption remains part of product success

The study reports 93.68% user satisfaction.

Even a technically strong optimization system provides little value if
operational users do not trust or use its recommendations.

---

## Critical Interpretation

The reported technical metrics should be treated carefully.

Values such as:

93.83% precision

and:

99.08% precision

do not by themselves establish the financial value of the system.

The stronger evidence comes from operational outcomes such as:

- Reduced driving time
- Reduced route distance
- Improved resource allocation

Future implementations should ideally measure additional business KPIs such
as:

- Fuel consumption
- Cost per delivery
- On-time delivery rate
- Vehicle utilization
- Deliveries per vehicle
- Cost per kilometer
- Failed deliveries
- Customer service level

---

## Gintech Relevance

This case is highly relevant to the Operations Intelligence opportunity.

It demonstrates a complete progression from historical operational data to
business action:

Business Data
        ↓
Predict
        ↓
Plan
        ↓
Optimize
        ↓
Recommend
        ↓
Execute
        ↓
Measure

This is closely aligned with the decision-intelligence architecture emerging
from the Gintech research.

---

## Potential Gintech Opportunity

Gintech should not necessarily build:

"AI Route Optimization"

as an isolated product.

A stronger concept would be:

**Logistics Decision Intelligence**

Potential workflow:

Orders
+
Historical Demand
+
Vehicles
+
Locations
+
Capacity
+
Delivery Constraints
        ↓
Expected Demand
        ↓
Operational Risk
        ↓
Resource Requirements
        ↓
Recommended Allocation
        ↓
Recommended Routes
        ↓
Operational Action

---

## Potential Inputs

A logistics intelligence product could potentially use:

- Historical orders
- Current orders
- Customer locations
- Delivery windows
- Vehicle availability
- Vehicle capacity
- Driver availability
- Historical travel times
- Inventory availability
- Distribution-center information

More advanced implementations could incorporate:

- Traffic
- Weather
- Fuel prices
- Real-time vehicle location
- Road restrictions
- Customer priority
- Service-level agreements

---

## Potential Outputs

Instead of simply presenting operational information, Gintech could
potentially generate:

- Expected demand
- Required logistics capacity
- Delivery-risk alerts
- Vehicle allocation recommendations
- Route recommendations
- Capacity utilization
- Expected driving time
- Expected delivery time
- Operational exceptions
- Priority actions

---

## Example Decision

Traditional Logistics Dashboard:

Orders today: 128
Vehicles available: 8
Pending deliveries: 43

Potential Decision Intelligence:

Orders today: 128
Expected capacity required: 9 vehicles
Available capacity: 8 vehicles

Risk:
Insufficient capacity for planned deliveries.

Expected impact:
12 deliveries at risk of missing target window.

Recommended Action:
Reallocate Vehicle 04 from Route B and move 7 low-priority deliveries to the
next available window.

The second output is much closer to an operational decision.

---

## Comparison With Ricoh

Ricoh:

Incident
        ↓
Predict Resolution Probability
        ↓
Remote vs On-Site Decision
        ↓
Operational Action

Héctor Ocaña:

Expected Demand
        ↓
Resource Planning
        ↓
Route Optimization
        ↓
Operational Action

Both cases demonstrate the same fundamental principle:

**Intelligence becomes valuable when connected to a repeatable operational
decision.**

---

## Comparison With Megatiendas

Megatiendas:

Historical Sales
        ↓
Demand Forecast
        ↓
Inventory Decision

Héctor Ocaña:

Historical Demand
        ↓
Demand Forecast
        ↓
Resource Planning
        ↓
Route Optimization
        ↓
Logistics Decision

This distinction is important.

Megatiendas primarily supports:

**What should we stock or purchase?**

Héctor Ocaña primarily supports:

**How should we deploy operational resources?**

Therefore, although both use demand forecasting, they represent different
decision domains.

---

## Regional Relevance

The case provides Latin American evidence that machine learning and
optimization can be combined to improve operational logistics decisions.

The specific results obtained in Peru should not automatically be assumed to
apply to companies in Colombia.

However, the decision pattern is transferable:

Demand
→ Capacity
→ Allocation
→ Routing
→ Delivery

This pattern can be investigated independently in logistics and distribution
companies in other Latin American markets.

---

## Potential MVP

A Gintech MVP would not need to reproduce the complete system.

A lower-complexity pilot could begin with:

Historical Orders
+
Delivery Data
+
Vehicle Data
        ↓
Operational Analysis
        ↓
Identify Inefficiencies
        ↓
Simple Recommendation Engine
        ↓
Measure Improvement

Only after demonstrating value would more advanced components such as:

- Machine learning demand forecasting
- Dynamic route optimization
- Real-time telemetry

need to be introduced.

This could significantly reduce the cost and complexity of initial
validation.

---

## Product Hypothesis

Can Gintech combine historical demand, order and logistics data to predict
operational requirements and recommend how companies should allocate
resources and execute deliveries more efficiently?

---

## Potential Gintech Capability

Primary:

Operations Intelligence

Supporting Capabilities:

- Demand Forecasting
- Logistics Analytics
- Resource Planning
- Route Optimization
- Operational Risk Detection
- Machine Learning
- Decision Support
- Business Intelligence

---

## Research Classification

Region:
Latin America

Country:
Peru

Industry:
Logistics / Transportation / Distribution

Primary Opportunity:
Operations Intelligence

Secondary Opportunity:
Demand Intelligence

Research Phase:
Regional Validation

---

## Evidence Strength

Primary source available:
Yes

Full PDF listed as open access:
Yes

Real organization:
Yes

Machine learning model:
Yes

Optimization component:
Yes

Integrated operational system:
Yes

Operational metrics:
Yes

User validation:
Yes

Long-term financial ROI demonstrated:
No

---

## Important Research Caution

The technical performance metrics reported by the thesis should not be
interpreted as equivalent business improvements.

The most useful evidence for Gintech is the demonstrated connection between:

Prediction
→ Optimization
→ Operational KPI

rather than the absolute model-performance percentages.

---

## Key Product Principle

Do not only predict what the operation will need.

Use the prediction to recommend how operational resources should respond.

---

## Status

Research completed
