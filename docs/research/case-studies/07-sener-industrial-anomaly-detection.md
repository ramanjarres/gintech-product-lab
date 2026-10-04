# Case Study: SENER Industrial Anomaly Detection

## Source

Company: SENER
Technology Partner: BigML
Domain: Industrial Operations / Anomaly Detection / Predictive Maintenance
Published: 2020
Use Case: Predicting oil temperature anomalies in Tunnel Boring Machines (TBMs)

Source:
Machine Learning in Construction: Predicting Oil Temperature Anomalies
in a Tunnel Boring Machine

---

## Business Context

SENER is an engineering and technology company operating across industries
including infrastructure, construction, energy, aerospace, transport,
oil and gas, and marine engineering.

One of its areas of expertise involves large-scale tunnel construction
using Tunnel Boring Machines (TBMs).

TBMs are extremely large and complex machines used to mechanically
excavate tunnels.

Because equipment failure can create significant operational delays and
costs, monitoring machine condition is an important part of tunnel
operations.

---

## Business Problem

One critical component of a Tunnel Boring Machine is its main bearing.

The bearing enables the cutter head to rotate and transfers the machine's
torque to the terrain.

The bearing requires continuous lubrication and can use thousands of
liters of oil.

Changes in lubricant oil temperature can indicate abnormal operating
conditions.

If these changes are not detected early, they can contribute to:

- Equipment wear
- Mechanical failure
- Unplanned downtime
- Higher maintenance costs
- Project delays
- Cost overruns

SENER wanted to determine whether machine learning could identify
operational conditions associated with oil temperature changes before
they became serious problems.

---

## Business Objective

The project had two main objectives:

1. Understand how internal TBM operating parameters relate to changes
   in oil temperature.

2. Predict temperature changes early enough to potentially avoid
   machinery wear or failure.

The objective therefore went beyond simply detecting an anomaly.

The system needed to provide enough warning for technicians to potentially
take preventive action.

---

## Data

The project used historical operational data from a previous SENER
tunneling project.

The dataset contained hundreds of measurements from the TBM.

Measurements were collected approximately every 10 seconds.

Examples of variables included:

- Torque
- Machine speed
- Pressure
- Chamber material characteristics
- Oil temperature
- Other internal machine parameters

This created a high-frequency industrial time-series dataset.

---

## Data Challenge

Significant oil temperature changes were relatively uncommon and
developed gradually.

This created an important machine learning challenge:

The dataset was highly imbalanced.

Most observations represented normal machine behavior while relatively
few observations represented conditions associated with significant
temperature increases.

Conceptually:

Normal Operation
████████████████████████████████

Potential Anomaly
██

A useful model therefore needed to identify rare but potentially
important patterns inside a very large amount of normal operational data.

---

## Machine Learning Approach

The project combined multiple analytical techniques rather than relying
on a single algorithm.

The workflow included:

1. Data exploration
2. Feature engineering
3. Association Discovery
4. Anomaly Detection
5. Classification
6. Operational evaluation

---

## Association Discovery

Association Discovery was used during data exploration.

The objective was to identify relationships between different operational
variables and temperature behavior.

This helped the team understand which combinations of machine conditions
might be associated with changes in oil temperature.

This step demonstrates that machine learning can also be used to discover
relationships in operational data before building a predictive model.

---

## Anomaly Detection

Anomaly Detection was used to identify unusual operational observations.

Instead of asking only:

"What does normal machine behavior look like?"

the system could also ask:

"Which observations behave differently from normal operating patterns?"

This is particularly useful in industrial environments where failures
are rare and historical examples may be limited.

---

## Classification

Classification models were then used to identify operational situations
associated with future temperature increases.

The combined approach allowed the team to isolate a subset of situations
where increases in oil temperature could be anticipated in advance.

The final objective was therefore predictive rather than purely
descriptive.

---

## Analytical Pipeline

The project can be represented conceptually as:

TBM Sensors
     ↓
Operational Data
     ↓
Data Exploration
     ↓
Feature Engineering
     ↓
Association Discovery
     ↓
Anomaly Detection
     ↓
Classification
     ↓
Potential Temperature Increase
     ↓
Early Warning
     ↓
Preventive Action

---

## Operationalization

The complete machine learning workflow was captured within the BigML
platform.

This allowed the process to support:

- Traceability
- Retraining
- Automation
- Repeatable model execution

This is important because industrial machine learning systems cannot
remain static.

New operational data continuously becomes available and models may need
to be retrained as operating conditions change.

---

## Business Value

The potential business value comes from identifying abnormal operating
conditions before they result in serious equipment problems.

Potential benefits include:

- Reduced equipment wear
- Fewer unexpected breakdowns
- Reduced downtime
- Better maintenance planning
- Lower operational costs
- Reduced project delay risk

The model therefore creates value only if its prediction leads to a
useful operational intervention.

---

## Key Findings

### 1. Industrial data can reveal early warning signals

Machines continuously generate operational data.

Patterns inside this data may provide warning signals before equipment
problems become visible through traditional monitoring.

---

### 2. Rare events create a different ML problem

Most machine observations represent normal behavior.

Failures and significant anomalies are comparatively rare.

This means traditional accuracy metrics can be misleading.

A model that predicts "normal" almost all the time could appear accurate
while failing to identify the events that actually matter.

---

### 3. Anomaly detection and prediction are different capabilities

Anomaly detection answers:

"Is something unusual happening?"

Prediction answers:

"What is likely to happen next?"

Combining both capabilities can provide more useful operational
intelligence.

---

### 4. Understanding relationships matters before prediction

Association Discovery helped identify relationships between machine
variables.

This shows the importance of understanding the operational system before
attempting to automate decisions.

---

### 5. The prediction must create time to act

Detecting a problem after equipment failure provides limited value.

The useful question is:

"Can we detect the conditions early enough for someone to intervene?"

This concept of actionable lead time is critical for predictive
maintenance.

---

### 6. Machine learning workflows require retraining

Industrial environments change.

Equipment ages, operating conditions change and new data becomes
available.

The project therefore included retraining and automation as part of the
workflow rather than treating the model as a one-time experiment.

---

## Gintech Relevance

This case introduces a potential Industrial Intelligence capability for
Gintech.

The same architecture does not necessarily require a Tunnel Boring
Machine.

Any company generating sufficient operational data could potentially use
similar principles.

Conceptually:

Operational Data
      ↓
Normal Behavior Baseline
      ↓
Anomaly Detection
      ↓
Risk Prediction
      ↓
Early Warning
      ↓
Recommended Action
      ↓
Business Outcome

---

## Potential Gintech Applications

### Manufacturing

Machine sensors
→ Detect abnormal behavior
→ Estimate failure risk
→ Recommend inspection or maintenance

### Industrial Operations

Operational measurements
→ Identify unusual process conditions
→ Alert operations teams
→ Prevent disruption

### Logistics

Vehicle or equipment telemetry
→ Detect abnormal performance
→ Predict maintenance requirements
→ Schedule preventive maintenance

### Energy

Equipment measurements
→ Detect operational anomalies
→ Identify potential equipment problems
→ Prioritize maintenance

### Telecom

Network and platform telemetry
→ Detect abnormal behavior
→ Identify emerging incidents
→ Prioritize investigation

The underlying principle remains similar even though the data source
changes.

---

## Potential Gintech Product Evolution

Stage 1:

Monitor

"What is happening?"

      ↓

Stage 2:

Detect

"Is something abnormal?"

      ↓

Stage 3:

Predict

"What might happen next?"

      ↓

Stage 4:

Recommend

"What should the business do?"

      ↓

Stage 5:

Measure

"Did the intervention prevent or reduce the problem?"

---

## Product Hypothesis

Can Gintech use operational data to detect abnormal behavior early,
estimate the risk of operational failure and recommend preventive action
before significant business impact occurs?

---

## Potential Gintech Capability

Industrial / Operations Intelligence

Supporting capabilities:

- Anomaly Detection
- Predictive Maintenance
- Operational Analytics
- Risk Prediction
- Decision Intelligence
- Automated Monitoring

---

## Key Product Principle

An anomaly is not automatically valuable information.

The value comes from detecting an abnormal condition early enough,
understanding its potential business impact and enabling an appropriate
response.

---

## Status

Research completed
