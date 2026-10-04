# Case Study: AI4Time Predictive Maintenance Analytics

## Source

Project: AI4Time
Institution: Corporación Unificada Nacional de Educación Superior (CUN)
Country: Colombia
Year: 2025
Industry: Hydrocarbons / Industrial Maintenance
Domain: Industrial Intelligence / Predictive Maintenance / Data Analytics

Authors:
- Yeimy Yesenia Garzón Abello
- Julián Andrés Nieto Sánchez
- Carlos Joaquín Parra Martínez

Source:
AI4Time: Estrategia en analítica de datos para el sector de mantenimiento industrial

Type:
Graduate specialization research project in Data Analytics

---

## Business Context

Industrial maintenance plays a critical role in industries such as
hydrocarbons, where equipment availability and reliability directly affect
operational continuity.

Organizations typically generate large amounts of maintenance information
through systems such as SAP PM.

This information can include:

- Maintenance orders
- Inspections
- Equipment history
- Failure records
- Maintenance activities
- Asset characteristics

However, historical maintenance data does not automatically translate into
better maintenance decisions.

AI4Time explored how historical maintenance information could be transformed
into predictive intelligence.

---

## Business Problem

Maintenance organizations frequently operate using preventive and corrective
maintenance strategies.

Corrective maintenance reacts after a failure occurs.

Preventive maintenance schedules interventions based on predefined intervals.

Both approaches can create inefficiencies when organizations cannot accurately
estimate the actual condition or failure risk of an asset.

The research identified several challenges including:

- Unplanned downtime
- Reactive decision making
- Poor information traceability
- Underutilized historical maintenance data
- High operational costs
- Difficulty anticipating equipment failures

The core opportunity was therefore to move from reactive maintenance toward
more proactive and data-driven maintenance decisions.

---

## Business Objective

The project aimed to improve predictive maintenance using historical
transactional maintenance data.

The main objectives included:

1. Characterize existing maintenance processes.
2. Improve data quality and governance.
3. Identify relevant maintenance KPIs.
4. Analyze equipment reliability.
5. Develop predictive models.
6. Estimate equipment Remaining Useful Life (RUL).
7. Create a decision-support dashboard.
8. Generate early-warning information for maintenance teams.

The ultimate objective was to transform historical maintenance data into
actionable operational intelligence.

---

## Data

The study analyzed information from more than:

**1,230 industrial assets**

registered in:

**SAP Plant Maintenance (SAP PM)**

covering the period:

**2020–2024**

The sample included equipment with different:

- Functional categories
- Criticality levels
- Maintenance frequencies

Historical information included maintenance transactions such as:

- Work orders
- Inspections
- Equipment records
- Maintenance events
- Failure information

---

## Data Quality Challenge

One of the most important limitations identified by the researchers was
data quality.

Historical maintenance records could contain:

- Missing information
- Inconsistent information
- Outdated records
- Data quality problems
- Poor traceability

This is particularly important because predictive models depend on the
quality of historical operational information.

The project therefore incorporated data governance and data quality as part
of the analytical process.

---

## Methodology

The project used the ASUM-DM methodology.

The process included stages related to:

1. Business understanding
2. Data understanding
3. Data preparation
4. Modeling
5. Evaluation
6. Implementation
7. Feedback and model improvement

This created an end-to-end analytical process rather than an isolated
machine learning experiment.

---

## Reliability Analysis

The project incorporated traditional reliability engineering techniques.

One of the main techniques used was the:

**Weibull distribution**

Weibull analysis can help understand equipment failure behavior and estimate
reliability characteristics.

This allowed the project to combine traditional engineering reliability
methods with machine learning.

---

## Machine Learning Approach

The project explored supervised machine learning techniques for both
classification and regression.

Random Forest was one of the principal algorithms used.

The models were designed to support tasks such as:

- Failure prediction
- Equipment condition analysis
- Remaining Useful Life estimation

Model performance was evaluated using metrics including:

- ROC
- AUC
- Precision
- Sensitivity
- MAE
- RMSE

---

## Remaining Useful Life

An important component of the project was estimating:

**Remaining Useful Life (RUL)**

Instead of simply asking:

"Has this machine failed?"

the system attempts to answer:

"How much useful operating life may remain before intervention becomes
necessary?"

Conceptually:

Historical Maintenance Data
        ↓
Asset Behavior
        ↓
Reliability Analysis
        ↓
Machine Learning
        ↓
Remaining Useful Life
        ↓
Maintenance Decision

This moves maintenance analytics from descriptive reporting toward
predictive decision support.

---

## Data Architecture

The project also included a data engineering component.

Data was processed and structured before being used for analytics and
visualization.

The implementation included:

- ETL processes
- SQL transformations
- Data Warehouse
- Star-schema data modeling
- Python-based analytics
- Power BI visualization

This is important because the predictive model represents only one component
of the complete solution.

---

## Dashboard

A functional dashboard prototype was developed using Power BI.

The dashboard included important maintenance KPIs such as:

- MTBF — Mean Time Between Failures
- MTTR — Mean Time To Repair
- Maintenance Backlog
- Early warnings
- Reliability indicators
- Historical and projected maintenance information

The dashboard acted as the interface between analytical models and maintenance
decision makers.

---

## Decision-Support Architecture

The AI4Time solution can be represented conceptually as:

SAP PM
   ↓
Historical Maintenance Data
   ↓
Data Quality & Governance
   ↓
ETL / Data Warehouse
   ↓
Reliability Analysis
   ↓
Machine Learning
   ↓
Failure / RUL Prediction
   ↓
Power BI
   ↓
Maintenance Decision
   ↓
Operational Action

---

## Validation

The project did not rely only on model evaluation.

Maintenance personnel were surveyed to understand:

- Current maintenance practices
- Existing operational needs
- Technology adoption
- Perceived usefulness of analytical tools

Technical workshops with maintenance experts were also used to provide
feedback and validate the solution.

This created an important combination of:

Technical Validation
+
User Validation

---

## Reported Operational Result

One particularly interesting reported result involved analytical processing
time.

Traditional equipment analysis performed using Excel could require more than:

**3 hours**

The automated analytical process using:

- ETL
- SQL transformations
- Python
- Machine Learning

reduced processing time to:

**less than 5 minutes**

for a volume exceeding 5,000 assets during the validation process.

This represents a significant improvement in analytical efficiency.

---

## Important Distinction

The reported reduction in analytical processing time should not be interpreted
as proof that equipment failures or maintenance costs were reduced by the same
magnitude.

The project demonstrates improvements in:

- Data processing
- Analytical capability
- Predictive modeling
- Maintenance visibility
- Decision support

but does not establish a complete long-term production ROI study showing
specific reductions in failures, downtime or maintenance expenditure.

---

## Key Findings

### 1. Valuable industrial data may already exist

Predictive maintenance does not always require building an IoT infrastructure
from scratch.

Organizations may already possess useful historical information inside
enterprise systems such as SAP PM.

---

### 2. Data quality can be a larger barrier than modeling

The project identified incomplete and inconsistent historical records as an
important limitation.

This means that a predictive maintenance product may first require:

Data Assessment
→ Data Cleaning
→ Data Governance
→ Analytics

before advanced machine learning becomes useful.

---

### 3. Traditional engineering and ML can complement each other

The project combined:

Weibull reliability analysis
+
Machine Learning

rather than treating machine learning as a replacement for established
engineering methods.

---

### 4. Prediction alone is not the product

The complete solution required:

Data
+
ETL
+
Data Warehouse
+
Statistical Analysis
+
Machine Learning
+
Dashboard
+
Business Workflow

The predictive model was only one layer.

---

### 5. The dashboard is an interface, not the intelligence itself

Power BI allowed maintenance teams to interact with:

- KPIs
- Predictions
- Alerts
- Reliability information

The value originated from the analytical pipeline behind the dashboard.

---

### 6. Human validation remains important

Maintenance experts participated in the validation process.

Domain expertise remains important when interpreting predictions and deciding
what maintenance action should be taken.

---

### 7. Existing enterprise systems can become intelligence sources

SAP PM was originally an operational maintenance system.

AI4Time demonstrates how information stored in operational systems can be
transformed into predictive intelligence.

This principle could potentially apply to:

- ERP
- CRM
- POS
- Ticketing systems
- Logistics platforms
- Inventory systems

---

## Limitations

The research identified several limitations.

### Data Quality

Historical records may contain missing, outdated or inconsistent information.

### Time and Resources

The project had limitations related to available research time and information.

### Broader Business Impact

The project did not fully evaluate areas such as:

- Occupational safety impact
- Environmental sustainability
- Long-term production ROI
- Organization-wide deployment

### Model Evolution

Future work could compare Random Forest with additional approaches such as:

- XGBoost
- Neural networks
- Hybrid reliability / ML models

---

## Gintech Relevance

This case is particularly relevant because it demonstrates a realistic
Colombian path from existing enterprise data to predictive decision support.

Gintech would not necessarily need to begin with sensor infrastructure.

A potential approach could be:

Existing Business System
        ↓
Historical Data
        ↓
Data Quality Assessment
        ↓
Data Model
        ↓
Analytics
        ↓
Prediction
        ↓
Dashboard
        ↓
Recommended Action

This lowers one of the barriers initially assumed for Industrial Intelligence.

---

## Potential Gintech Opportunity

A potential Gintech industrial product could begin as an analytics layer on
top of existing maintenance systems.

Instead of:

"Install hundreds of sensors and build an IoT platform"

an initial proposition could be:

"Use the maintenance data you already have to identify operational risks and
improve maintenance decisions."

This could significantly reduce the complexity of an initial pilot.

---

## Potential Applications Beyond Hydrocarbons

The architecture could potentially apply to organizations with asset and
maintenance histories in areas such as:

### Manufacturing

Maintenance history
→ Reliability analysis
→ Failure risk
→ Maintenance recommendation

### Logistics

Fleet maintenance records
→ Vehicle reliability
→ Maintenance risk
→ Intervention prioritization

### Utilities

Asset history
→ Reliability analysis
→ Risk prediction
→ Preventive intervention

### Industrial Services

Work orders
→ Equipment history
→ Failure patterns
→ Maintenance planning

---

## Product Hypothesis

Can Gintech transform maintenance data that companies already store in
enterprise systems into predictive intelligence that helps prioritize
maintenance interventions before operational disruption occurs?

---

## Potential Gintech Capability

Industrial / Operations Intelligence

Supporting capabilities:

- Data Quality
- Data Engineering
- Reliability Analytics
- Predictive Maintenance
- Remaining Useful Life
- Machine Learning
- Business Intelligence
- Decision Support

---

## Comparison With SENER

SENER:

Sensor / Machine Data
→ Detect abnormal behavior
→ Predict temperature change
→ Preventive intervention

AI4Time:

Enterprise Maintenance Data
→ Reliability analysis
→ Predict failure / RUL
→ Prioritize maintenance

The difference is strategically important.

SENER suggests an IoT / sensor-heavy path.

AI4Time suggests that predictive industrial intelligence may also be possible
using historical enterprise data that companies already possess.

---

## Key Product Principle

Before asking a company to generate new data, determine whether valuable
operational intelligence can be extracted from the data it already owns.

---

## Research Classification

Region: Colombia / Latin America

Primary Opportunity:
Industrial Intelligence

Secondary Opportunity:
Operations Intelligence

Research Phase:
Regional Validation

---

## Status

Research completed
