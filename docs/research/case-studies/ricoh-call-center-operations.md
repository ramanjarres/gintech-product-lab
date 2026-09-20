# Case Study: Ricoh Call Center Operations Optimization

## Source

Company: Ricoh  
Solution Partner: Clever Data  
Domain: Operations Intelligence / Customer Support / Machine Learning  
Initial Project Period: 2017  
Use Case: Incident routing and remote-resolution prediction

---

## Business Problem

Ricoh operates an after-sales support service for printers and other
office equipment.

Customer incidents could enter the system through different channels,
including web forms, call centers, and devices capable of automatically
reporting incidents.

A dispatch engineer reviewed each incident and decided whether it should:

1. Be handled remotely by the help desk.
2. Require an engineer to visit the customer's location.

On-site repair was significantly more expensive than remote resolution.

Ricoh therefore wanted to increase its "visit avoidance" KPI by identifying
more incidents that could successfully be resolved remotely.

---

## Business Objective

Increase the percentage of incidents successfully resolved remotely while
reducing unnecessary on-site technician visits.

The goal was not simply to classify support tickets.

The system needed to support an operational decision:

> Should this incident be handled remotely or require an on-site visit?

---

## Existing Process

Incident created
        ↓
CRM
        ↓
Dispatch Engineer
        ↓
Incident review
        ↓
Decision
   ↙             ↘
Remote          On-site
Support         Technician

The decision depended heavily on the dispatch engineer's experience and
interpretation of the incident description.

---

## Data

The original historical dataset contained approximately:

- 150,000 incidents
- January 2016 – July 2017
- 61 variables per incident

Available information included:

- Printer characteristics
- Printer model
- Device capabilities
- Customer/contact information
- Incident description
- Technical characteristics
- Historical resolution outcome
- Whether the incident was resolved remotely

The incident description was particularly important because it contained
unstructured free text describing the problem.

Examples included:

- Paper jams
- Network problems
- Printing defects
- Black lines on printed documents
- Device failures

---

## Data Preparation

After data exploration, cleaning and feature engineering, the dataset used
for model development was reduced to approximately:

- 40,000 incidents
- March 2017 – July 2017
- 25 variables

This highlights an important lesson:

Most of the original data was not automatically useful for modeling.

The team emphasized that data understanding, cleaning and feature
engineering represented approximately 90–95% of the machine learning
project effort.

---

## Machine Learning Approach

The solution combined unsupervised and supervised machine learning.

### Step 1 — Topic Modeling

Approximately 40,000 incident descriptions were processed using topic
modeling.

The objective was to discover what customers were describing in their
incident reports.

Examples of discovered topics included:

- Paper jams
- Printing lines
- Tray problems
- Reboot issues
- Other printer-related failures

Topic modeling transformed unstructured text into structured information.

---

## Step 2 — Feature Enrichment

The topics identified in the incident description were added as new
features to each incident.

The dataset therefore evolved from:

Device characteristics + incident description

to:

Device characteristics
+
incident description
+
topic information

The unsupervised model was therefore not the final decision engine.

Its role was to enrich the dataset.

---

## Step 3 — Supervised Prediction

The enriched dataset was divided into training and test data.

Multiple machine learning models and configurations were evaluated.

A Random Forest ensemble was selected as the production model.

The model predicted whether an incident should be:

- Handled remotely
- Sent for on-site repair

---

## Prediction Pipeline

When a new incident arrived:

New incident
      ↓
Incident description
      ↓
Topic modeling
      ↓
Topic features
      ↓
Combined with device and incident data
      ↓
Random Forest
      ↓
Remote vs On-site recommendation

---

## Example

Incident description:

"Constantly jamming in right-hand side, cleared several times."

The topic model identified the incident as primarily related to:

1. Paper/jamming
2. Printing/page problems
3. Reboot-related issues

This information was added to the incident before the final prediction.

---

## Implementation

The solution was implemented through:

- Backend services
- Authentication
- Machine learning module
- API
- Web interface for manual predictions

The system could therefore integrate with Ricoh's operational workflow
while also allowing employees to request individual predictions manually.

The solution was initially deployed in Spain and later expanded to other
European markets.

---

## Business Results

The most important result was not model accuracy.

Ricoh measured the operational outcome.

Before implementation:

Approximately 61% of incidents selected for remote handling were
successfully resolved remotely.

After implementation:

Approximately 81% were successfully resolved remotely.

This represents an improvement of roughly 20 percentage points.

The business impact came from avoiding unnecessary technician visits and
therefore reducing operational costs.

---

## Key Findings

### 1. Start with the business decision

The project did not begin with:

"How can Ricoh use topic modeling?"

It began with:

"How can Ricoh reduce unnecessary technician visits?"

Machine learning was selected because there was a repeatable operational
decision that could be supported using historical data.

---

### 2. Unstructured customer data can become operational data

Incident descriptions initially existed as free text.

Topic modeling converted that information into structured features that
could be used by another predictive model.

Unstructured text therefore became part of an operational decision system.

---

### 3. Unsupervised and supervised ML can work together

Topic modeling:

Discover and structure information.

Random Forest:

Predict an operational outcome.

The value came from the complete pipeline rather than from either model
individually.

---

### 4. Data preparation dominates the work

The project started with approximately:

150,000 incidents × 61 variables

and ultimately modeled approximately:

40,000 incidents × 25 variables.

Understanding, cleaning and transforming the data represented most of the
project effort.

---

### 5. Business KPIs matter more than model KPIs

The project team explicitly emphasized business outcomes over metrics such
as accuracy, recall or precision.

The relevant question was not:

"How accurate is the Random Forest?"

The relevant question was:

"Are more incidents successfully resolved remotely?"

---

### 6. Machine learning should support a decision

The system was inserted at a specific decision point in an existing
business process.

This made the model actionable.

Prediction without integration into the operational workflow would have
provided significantly less value.

---

### 7. Machine learning systems require continuous improvement

The team described the ML lifecycle as iterative.

New data, changes in data quality, additional variables and new modeling
techniques require models to be periodically reviewed and retrained.

---

## Gintech Relevance

This case is highly relevant to Gintech because it demonstrates how
customer and operational data can be transformed into decision support.

A potential Gintech architecture could follow the same pattern:

Business Data
      ↓
Unstructured Information
      ↓
Information Extraction
      ↓
Structured Features
      ↓
Prediction
      ↓
Business Decision
      ↓
Measured Outcome

---

## Potential Gintech Applications

The same pattern could potentially be adapted to:

### Customer Support

Ticket
→ Understand issue
→ Predict resolution path
→ Recommend team/action

### Telecom

Customer interaction
→ Detect issue
→ Combine with journey/account data
→ Predict escalation or resolution path
→ Recommend intervention

### Retail

Customer complaint
→ Identify issue
→ Combine with transaction/store data
→ Predict operational cause or risk
→ Recommend action

### Industrial Operations

Maintenance report
→ Extract failure information
→ Combine with machine data
→ Predict maintenance requirement
→ Recommend intervention

### Restaurants

Customer complaint/order issue
→ Identify problem
→ Combine with order/location data
→ Predict operational source
→ Recommend corrective action

---

## Product Hypothesis

Can Gintech combine unstructured business information with operational
data to predict the best action for a recurring business decision?

---

## Potential Gintech Capability

Operations Intelligence

Supporting capabilities:

- Customer Intelligence
- NLP
- Decision Intelligence
- Predictive Analytics
- Workflow Optimization

---

## Key Product Principle

Do not build machine learning models simply to generate predictions.

Build systems that improve measurable business decisions.

---

## Status

Research completed
