# Gintech Product Lab — Opportunity Evaluation Matrix

## Purpose

This document compares the initial opportunity areas identified during
Gintech Product Lab research.

The objective is to determine which problem space should be prioritized
for further validation and potentially selected as the initial target
segment for the Product Lab.

This matrix is not a final market selection.

The current scores represent initial hypotheses based on:

- Case study research
- Expected data availability
- Expected customer accessibility
- MVP feasibility
- Technical requirements
- Potential business impact

These assumptions must be validated with market research, real datasets
and potential customer interviews.

---

## Status

**Stage:** Initial Opportunity Evaluation  
**Version:** 1.0  
**Decision Status:** No target segment selected yet

---

## Research Foundation

Four real-world implementations were reviewed before creating this
matrix.

| Company | Intelligence Area | Core Problem |
|---|---|---|
| Airbnb | Customer Intelligence | Understand and classify customer message intent |
| Ricoh | Operations Intelligence | Predict the appropriate resolution path for service incidents |
| Nestlé | Demand Intelligence | Forecast sell-in and sell-out demand |
| SENER | Industrial Intelligence | Detect and anticipate abnormal equipment behavior |

Detailed research:

- `docs/research/case-studies/airbnb-message-intent-classification.md`
- `docs/research/case-studies/ricoh-call-center-operations.md`
- `docs/research/case-studies/nestle-demand-forecasting.md`
- `docs/research/case-studies/sener-industrial-anomaly-detection.md`

---

## Common Pattern Identified

Although the four companies address different problems, their solutions
share a common pattern:

Business Data
      ↓
Understand
      ↓
Detect / Predict
      ↓
Assess Business Impact
      ↓
Support a Decision
      ↓
Take Action
      ↓
Measure Outcome

This suggests that Gintech should explore decision-support capabilities
rather than isolated dashboards or machine learning models.

---

# Candidate Opportunity Areas

## 1. Customer Intelligence

### Problem

Companies receive large amounts of unstructured customer information but
often struggle to convert it into actionable insights.

Potential data sources include:

- Surveys
- Reviews
- Support tickets
- Chats
- Call transcripts
- Customer complaints
- Social feedback

### Potential Capability

Transform unstructured customer feedback into structured intelligence.

Potential outputs:

- Topic
- Intent
- Sentiment
- Severity
- Frequency
- Emerging issues
- Business impact
- Recommended actions

### Reference Case

Airbnb — Message Intent Classification

---

## 2. Operations Intelligence

### Problem

Businesses make repetitive operational decisions that depend on employee
experience, manual analysis or fragmented information.

Potential examples:

- Ticket routing
- Incident prioritization
- Escalation decisions
- Service resolution
- Operational risk detection
- Workflow prioritization

### Potential Capability

Use historical operational data to support or automate recurring business
decisions.

### Reference Case

Ricoh — Call Center Operations Optimization

---

## 3. Demand Intelligence

### Problem

Companies need to anticipate future demand to make better decisions about:

- Inventory
- Purchasing
- Production
- Staffing
- Distribution
- Financial planning

### Potential Capability

Use historical sales and operational data to forecast future demand and
translate predictions into business recommendations.

### Reference Case

Nestlé — Sell-In & Sell-Out Demand Forecasting

---

## 4. Industrial Intelligence

### Problem

Industrial companies generate operational and equipment data but may not
identify abnormal behavior early enough to prevent disruption.

Potential data sources include:

- Sensors
- Equipment telemetry
- Maintenance records
- Production systems
- Operational measurements

### Potential Capability

Detect abnormal operating conditions, estimate operational risk and
support preventive intervention.

### Reference Case

SENER — Industrial Anomaly Detection

---

# Evaluation Method

Each opportunity is evaluated using a score from 1 to 5.

| Score | Meaning |
|---|---|
| 1 | Very unfavorable |
| 2 | Unfavorable |
| 3 | Moderate / uncertain |
| 4 | Favorable |
| 5 | Very favorable |

Scores in this version represent hypotheses.

They should change when new evidence becomes available.

---

# Evaluation Criteria

## Problem Frequency — 10%

How frequently does the problem occur for potential customers?

A recurring problem provides more opportunities to demonstrate continuous
value.

---

## Business Impact — 15%

How strongly can solving the problem affect:

- Revenue
- Cost
- Productivity
- Customer experience
- Operational risk

High-impact problems are more likely to receive business attention.

---

## Data Availability — 15%

How likely is it that potential customers already possess the data
required to build the solution?

Examples:

- Transaction history
- Customer feedback
- Operational events
- Inventory records
- Sensor data

---

## Access to Customers — 15%

How easily can Gintech reach organizations experiencing the problem?

This includes:

- Existing relationships
- Local businesses
- Industry contacts
- Potential pilot customers
- Decision-maker accessibility

---

## MVP Feasibility — 15%

Can Gintech build a useful first version without requiring excessive:

- Infrastructure
- Integration
- Data engineering
- Specialized hardware
- Capital
- Development time

---

## Time to Value — 10%

How quickly could a customer observe measurable value after implementation?

Shorter time to value may simplify early product validation.

---

## Technical Complexity — 5%

How difficult would the initial solution be to develop and maintain?

A higher score means lower technical barriers for an initial MVP.

---

## Validation With Real Data — 10%

How easily can Gintech obtain sufficient real or realistic data to test
the hypothesis?

---

## Potential Willingness to Pay — 5%

How likely is the problem to justify paying for a solution?

This score remains highly uncertain until customer interviews and market
research are completed.

---

# Opportunity Evaluation Matrix — Version 1

| Criteria | Weight | Customer Intelligence | Operations Intelligence | Demand Intelligence | Industrial Intelligence |
|---|---:|---:|---:|---:|---:|
| Problem Frequency | 10% | 5 | 5 | 5 | 4 |
| Business Impact | 15% | 4 | 5 | 5 | 5 |
| Data Availability | 15% | 5 | 4 | 4 | 2 |
| Access to Customers | 15% | 5 | 4 | 4 | 2 |
| MVP Feasibility | 15% | 5 | 4 | 4 | 2 |
| Time to Value | 10% | 5 | 4 | 4 | 3 |
| Technical Complexity | 5% | 4 | 3 | 3 | 1 |
| Validation With Real Data | 10% | 5 | 4 | 4 | 2 |
| Potential Willingness to Pay | 5% | 3 | 4 | 4 | 5 |
| **Weighted Score** | **100%** | **4.65** | **4.20** | **4.15** | **2.70** |

---

# Initial Interpretation

## Customer Intelligence — 4.65 / 5

### Strengths

Customer data can potentially be obtained from relatively accessible
sources such as reviews, surveys, support interactions and customer
feedback.

An MVP could potentially be developed without complex infrastructure.

The main opportunity is not simply sentiment analysis.

A stronger product hypothesis would connect customer signals with:

- Issue detection
- Prioritization
- Business impact
- Recommended action

### Main Risk

The market already contains many customer analytics, sentiment analysis
and Voice of Customer tools.

Gintech would need to demonstrate differentiation beyond summarizing or
classifying feedback.

### Current Assessment

**Promising — requires differentiation validation**

---

## Operations Intelligence — 4.20 / 5

### Strengths

Operational decisions happen continuously inside businesses.

Examples include:

- Prioritization
- Routing
- Escalation
- Resource allocation
- Incident resolution

Improving a repeated decision can create measurable operational value.

### Main Risk

Operational processes vary significantly between companies.

A solution could become overly customized if a common repeatable problem
is not identified.

### Current Assessment

**Promising — requires problem standardization research**

---

## Demand Intelligence — 4.15 / 5

### Strengths

Demand forecasting can directly influence:

- Inventory
- Purchasing
- Production
- Staffing
- Distribution
- Financial planning

Historical transaction data may already exist within many companies.

### Main Risk

Useful forecasting requires sufficient historical data and reasonable data
quality.

Small companies may not have enough structured history to produce reliable
forecasts.

### Current Assessment

**Promising — requires data availability validation**

---

## Industrial Intelligence — 2.70 / 5

### Strengths

Industrial failures and operational disruption can create significant
financial impact.

This may create strong willingness to pay when a solution can reliably
reduce risk.

### Main Risk

Initial implementation may require:

- Sensor data
- Equipment integrations
- Industrial domain expertise
- Large historical datasets
- Access to engineering teams
- Longer validation cycles

These requirements create significant barriers for an early Gintech MVP.

### Current Assessment

**High potential value — high initial entry barrier**

---

# Important Limitation

The weighted scores should not be interpreted as market facts.

For example:

Customer Intelligence scoring 4.65 does not prove that it is the best
market for Gintech.

It currently means:

> Based on our present assumptions, Customer Intelligence appears easier
> to validate and build as an initial product.

Market evidence may change this conclusion.

---

# Emerging Product Architecture

The research suggests a possible common architecture across multiple
opportunity areas.

Data
  ↓
Understand
  ↓
Detect / Predict
  ↓
Assess Impact
  ↓
Recommend
  ↓
Act
  ↓
Measure

Examples:

Customer Intelligence:

Customer Feedback
→ Detect Issue
→ Prioritize
→ Recommend Action

Operations Intelligence:

Operational Events
→ Predict Outcome
→ Recommend Decision

Demand Intelligence:

Sales Data
→ Forecast Demand
→ Identify Risk
→ Recommend Action

Industrial Intelligence:

Sensor Data
→ Detect Anomaly
→ Estimate Risk
→ Recommend Intervention

This architecture is currently a research hypothesis and should not yet
be considered the final Gintech product architecture.

---

# Opportunities Moving Forward

Based on the initial evaluation, three areas should continue to the next
validation stage:

1. Customer Intelligence
2. Operations Intelligence
3. Demand Intelligence

Industrial Intelligence should remain in the research backlog because of
its potential business value, but its initial entry barriers currently
appear significantly higher.

This is not a final product selection.

---

# Next Validation Stage

The next phase should replace assumptions with evidence.

For each shortlisted opportunity, research should evaluate:

- Who experiences the problem?
- How frequently does it occur?
- How is it solved today?
- What does the current problem cost?
- What data is available?
- Who owns the data?
- Who makes the purchasing decision?
- What existing tools are used?
- What are customers currently paying?
- What would prevent adoption?
- Can Gintech demonstrate value with a small pilot?

---

# Validation Evidence

Evidence should be collected from:

- Market research
- Public datasets
- Industry reports
- Potential customer interviews
- Existing software solutions
- Competitor analysis
- Pilot datasets
- Business process observations

Each new piece of evidence should be used to review the matrix scores.

---

# Decision Rule

The initial Gintech Product Lab segment should not be selected solely
because it has the highest numerical score.

The final decision should consider:

**Market attractiveness
+ Problem severity
+ Data accessibility
+ Customer accessibility
+ MVP feasibility
+ Ability to demonstrate measurable value**

The selected opportunity should have both a meaningful business problem
and a realistic path to validation.

---

# Next Step

Conduct market validation for the three shortlisted opportunities:

- Customer Intelligence
- Operations Intelligence
- Demand Intelligence

Use the collected evidence to create:

**Opportunity Evaluation Matrix — Version 2**

The Version 2 matrix will be used to support the initial target segment
decision.

---

## Status

Initial opportunity evaluation completed.

Target segment selection pending market validation.
