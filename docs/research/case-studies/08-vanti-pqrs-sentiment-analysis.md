# Case Study: Vanti PQRS Sentiment Analysis

## Source

Project:
Development of Natural Language Processing Models Using Machine Learning
Techniques for Sentiment Analysis of Industrial Customer PQRS at Vanti S.A. ESP

Organization:
Vanti S.A. ESP

Institution:
Universidad EAN

Country:
Colombia

Year:
2026

Industry:
Utilities / Natural Gas / B2B Customer Service

Domain:
Customer Intelligence / NLP / Voice of Customer

Author:
Juan Sebastián Lozano Forero

Academic Program:
Master's Degree in Data Science

Primary Source:
https://repository.universidadean.edu.co/entities/publication/f74b3e51-773a-4e10-ae13-fc845a30e743/full

Full Document:
https://repository.universidadean.edu.co/bitstreams/8e361075-fcdf-40cb-a021-9196cc42624e/download

---

## Business Context

Vanti receives Petitions, Complaints, Claims and Suggestions (PQRS) from
industrial customers through its customer service processes.

These interactions contain valuable information about:

- Customer dissatisfaction
- Service problems
- Administrative requests
- Payment-related situations
- Operational issues
- Customer expectations
- Potential critical cases

However, much of this information exists as unstructured text.

The organization therefore possesses valuable Voice of Customer information,
but extracting patterns and insights from it requires significant manual
analysis.

---

## Business Problem

The existing PQRS management process relied heavily on manual handling and
analysis of customer communications.

This created several limitations:

- Manual review of customer interactions
- Difficulty analyzing large volumes of text
- Limited ability to identify emotional tone
- Difficulty detecting patterns of dissatisfaction
- Slow identification of critical cases
- Underutilization of historical customer information

The fundamental problem was therefore not the absence of customer data.

The problem was the organization's limited ability to transform unstructured
customer feedback into useful information for decision-making.

---

## Business Objective

The project aimed to develop a Natural Language Processing model capable of
automatically classifying industrial customer PQRS according to sentiment.

The target categories were:

- Positive
- Neutral
- Negative

The broader objective was to transform unstructured customer communications
into structured information that could support:

- Customer service analysis
- Identification of critical cases
- Detection of dissatisfaction
- Strategic decision-making
- Customer experience improvement

---

## Organizational Diagnosis

Before developing the model, the research evaluated the existing PQRS
management process.

The diagnosis considered:

- Existing operational procedures
- Manual information management
- Time required to review customer requests
- Availability of historical data
- Technological support
- Employee perception
- Customer service processes

This is an important characteristic of the project.

The research did not begin with:

"Which machine learning model should we use?"

It began with:

"How does the organization currently manage this business problem?"

---

## Data

The project used historical PQRS information from industrial customers.

One of the most important variables was:

**Observations**

This field contained the unstructured text describing the customer
interaction.

The dataset also contained additional information related to the customer
service process.

The text records varied significantly in length and quality.

Examples of data-quality problems included:

- Missing values
- Very short texts
- Administrative codes
- Alphanumeric identifiers
- Noise
- Special characters
- Non-semantic records
- Inconsistent language

The text therefore required significant preprocessing before modeling.

---

## Data Quality

Data quality became an important component of the project.

Some dataset fields contained substantial missing information.

The Observations field, however, contained information for approximately
99.9% of the analyzed records, making it particularly valuable for the NLP
analysis.

Text length varied considerably.

The average text contained approximately 271 characters, while some records
contained only a single character and others exceeded 12,000 characters.

Examples of low-quality records included values such as:

"C"
"1"
"0"
"."

These records contained little or no useful semantic information.

---

## Methodology

The research followed a structured analytical process.

### Phase 1 — Business Understanding

Understand the PQRS process and identify the business opportunity.

### Phase 2 — Data Exploration

Analyze:

- Dataset structure
- Missing values
- Text length
- Word frequency
- Bigrams
- Trigrams
- Non-significant records

### Phase 3 — Data Preparation

Perform:

- Text cleaning
- Normalization
- Removal of irrelevant records
- Special-character processing
- Noise reduction

### Phase 4 — Target Variable Construction

Create sentiment labels using a hybrid approach.

### Phase 5 — Text Vectorization

Transform text into numerical features using TF-IDF.

### Phase 6 — Feature-Space Analysis

Use techniques such as t-SNE to understand the distribution and semantic
overlap between classes.

### Phase 7 — Machine Learning

Train and compare classification models.

### Phase 8 — Model Evaluation

Evaluate model performance using multiple classification metrics.

### Phase 9 — Implementation

Integrate preprocessing, TF-IDF and the selected model into a proposed
operational workflow.

---

## Sentiment Labeling Strategy

One of the most interesting parts of the project was the construction of the
target variable.

The historical PQRS data did not already contain reliable sentiment labels.

The researchers therefore created a hybrid labeling system.

The process combined:

### Domain Dictionary

A dictionary was created using real positive and negative expressions from
Vanti customer interactions.

### VADER

VADER sentiment analysis was used as an additional signal.

Because VADER was originally designed primarily for English, it was not used
as the principal labeling mechanism.

Instead, it was used mainly as a secondary layer for ambiguous situations.

### Business Rules

The final layer incorporated urgency criteria based on business context.

Conceptually:

Customer Text
      ↓
Domain Dictionary
      ↓
VADER
      ↓
Business Rules / Urgency
      ↓
Sentiment Label

This produced the target variable used to train the supervised models.

---

## Text Representation

The project used:

**TF-IDF — Term Frequency–Inverse Document Frequency**

to transform customer text into numerical features.

Conceptually:

Customer PQRS
      ↓
Text Cleaning
      ↓
TF-IDF
      ↓
Numerical Feature Vector
      ↓
Machine Learning Model

---

## Machine Learning

Multiple classification approaches were evaluated.

The strongest model was:

**Linear Support Vector Machine (Linear SVM)**

Linear SVM showed the strongest overall performance, particularly in:

- Macro F1-score
- Cross-validation stability
- Class discrimination

The model was selected as the proposed classifier for sentiment analysis.

---

## Model Results

The selected Linear SVM model demonstrated strong overall ability to
distinguish between sentiment categories.

Reported AUC values included approximately:

Positive:
0.978

Neutral:
0.948

Negative:
0.930

These results indicate strong class-discrimination capability within the
analyzed dataset.

However, aggregate metrics do not tell the complete story.

---

## Important Model Limitation

The confusion matrix revealed an important business risk.

Approximately:

**21% of negative records were classified as neutral**

in the analyzed evaluation.

This is particularly important because negative customer interactions may
represent the cases where intervention is most valuable.

Therefore:

High Overall Model Performance

does not automatically mean:

Low Business Risk

A false negative or negative-to-neutral classification could cause a
potentially important customer problem to receive insufficient attention.

---

## Business Interpretation

This creates an important distinction between:

### Model Metric

How accurately does the model classify sentiment?

and:

### Business Metric

How effectively does the system identify customer situations requiring
attention?

For Customer Intelligence, these are not necessarily the same objective.

A model could have strong overall performance while still missing customer
interactions that are operationally important.

---

## Model Explainability

The Linear SVM model also allowed the researchers to inspect terms strongly
associated with each sentiment category.

Examples associated with negative sentiment included terms related to:

- Dissatisfaction
- Suspension
- Service interruption

Neutral interactions contained more language associated with:

- Requests
- Payment agreements
- Administrative processes

Positive interactions contained terms associated with:

- Acceptance
- Gratitude
- Agreement
- Satisfaction

This provided additional interpretability beyond the final sentiment label.

---

## Implementation

The proposed implementation combined:

Customer PQRS
      ↓
Text Preprocessing
      ↓
TF-IDF
      ↓
Linear SVM
      ↓
Sentiment Prediction
      ↓
Interpretation
      ↓
Customer Service Analysis

The model was designed as a decision-support tool rather than a replacement
for customer service personnel.

---

## Human-in-the-Loop

The research explicitly recognizes that the objective of the system is not
to replace human judgment.

Instead, the system should strengthen the analytical and operational
capabilities of employees responsible for PQRS management.

This creates a human-in-the-loop architecture:

AI Classification
      ↓
Prioritization / Insight
      ↓
Human Review
      ↓
Business Decision
      ↓
Customer Action

---

## Production Considerations

The project also considered what would be required beyond model development.

These included:

- User adoption
- Training
- Data quality monitoring
- Infrastructure
- Model monitoring
- Model retraining
- Information security
- Governance
- Production performance measurement

This makes the case particularly valuable because it recognizes that model
development is only one component of an operational AI system.

---

## Risks

The research identified several important implementation risks.

### User Adoption

Employees may not adopt the analytical system.

Mitigation includes:

- Training
- Workshops
- Dashboard support
- Change management

### Data Quality

PQRS information may contain:

- Missing values
- Noise
- Ambiguous language
- Abbreviations

Continuous validation and cleaning are therefore required.

### Model Drift

Customer language and interaction patterns may change over time.

The model may therefore lose predictive performance.

Continuous monitoring and periodic retraining are required.

### Infrastructure

The organization requires sufficient technological infrastructure to operate
the solution reliably.

### Privacy and Security

Customer information requires appropriate:

- Access controls
- Secure storage
- Governance
- Data protection

---

## Key Findings

### 1. Customer feedback is operational data

PQRS should not be treated only as individual customer-service records.

At scale, they form a dataset capable of revealing recurring customer
problems and patterns.

---

### 2. Unstructured data can become structured intelligence

The project transformed:

Customer Text

into:

Sentiment Category

This creates structured information that can be aggregated, analyzed and
monitored.

---

### 3. Domain knowledge matters

Generic sentiment tools were not sufficient.

The researchers incorporated:

- Vanti-specific language
- Domain dictionaries
- Business urgency rules

This suggests that useful Customer Intelligence requires understanding the
language and context of the organization.

---

### 4. Accuracy is not enough

Misclassifying negative interactions as neutral demonstrates why model
evaluation should consider business consequences.

For example:

Negative → Neutral

may be more costly than:

Positive → Neutral

The model should therefore eventually be evaluated according to the business
impact of different errors.

---

### 5. Sentiment is useful but incomplete

Sentiment tells the organization:

"How does this interaction sound?"

It does not necessarily tell the organization:

"What problem is the customer experiencing?"

or:

"What should the organization do next?"

This represents an important opportunity for a more advanced Customer
Intelligence product.

---

## Critical Gintech Interpretation

Gintech should **not** simply reproduce the Vanti solution as:

PQRS
→ Sentiment Analysis
→ Dashboard

Sentiment analysis is increasingly accessible and by itself may provide
limited differentiation.

A stronger architecture would move beyond sentiment.

For example:

Customer Interaction
        ↓
What happened?
        ↓
What problem is being reported?
        ↓
How severe is it?
        ↓
How frequently is it occurring?
        ↓
Which customers are affected?
        ↓
What business process is involved?
        ↓
What action should be prioritized?

Sentiment becomes one signal among several.

---

## Potential Gintech Customer Intelligence Architecture

Potential inputs:

- PQRS
- Customer support tickets
- Call-center transcripts
- Surveys
- Reviews
- Emails
- Chat conversations
- WhatsApp conversations

Potential intelligence layer:

- Sentiment
- Intent
- Issue classification
- Topic detection
- Severity
- Frequency
- Recurrence
- Customer segment
- Business impact

Potential output:

Customer Problem
        ↓
Severity
        ↓
Affected Customers
        ↓
Frequency
        ↓
Business Impact
        ↓
Recommended Priority
        ↓
Recommended Action

---

## Comparison With Airbnb

Airbnb:

Customer Messages
        ↓
Topic Discovery
        ↓
Intent Taxonomy
        ↓
Intent Classification
        ↓
Customer / Support Action

Vanti:

Customer PQRS
        ↓
Sentiment Labeling
        ↓
Sentiment Classification
        ↓
Critical Case Identification
        ↓
Customer Service Analysis

Airbnb focuses primarily on:

**What does the customer need?**

Vanti focuses primarily on:

**What sentiment does the customer express?**

A potential Gintech product could combine both:

What happened?
+
What does the customer need?
+
How serious is it?
+
How frequently is it happening?
+
What should the business do?

---

## Connection With Gintech Research

This case provides regional evidence for the Customer Intelligence
opportunity.

It demonstrates that a Colombian organization can already possess valuable
unstructured customer information but still face difficulties converting
that information into timely analytical insight.

This reinforces the hypothesis that the opportunity may not be collecting
more customer feedback.

The opportunity may be extracting more value from feedback that companies
already collect.

---

## Potential Gintech Opportunity

A potential initial product proposition could be:

"Transform the customer interactions your company already receives into
prioritized business problems and recommended actions."

Rather than:

"Analyze customer sentiment with AI."

This distinction is strategically important.

---

## Product Hypothesis

Can Gintech transform existing customer interactions into structured
intelligence that automatically identifies recurring problems, measures their
severity and frequency, and helps organizations prioritize the actions with
the greatest customer and business impact?

---

## Potential Gintech Capability

Primary:

Customer Intelligence

Supporting Capabilities:

- Voice of Customer
- Natural Language Processing
- Sentiment Analysis
- Intent Classification
- Issue Detection
- Topic Classification
- Severity Detection
- Prioritization
- Decision Support

---

## Research Classification

Region:
Colombia / Latin America

Industry:
Utilities / B2B Customer Service

Primary Opportunity:
Customer Intelligence

Secondary Opportunity:
Operations Intelligence

Research Phase:
Regional Validation

---

## Evidence Strength

Primary source available:
Yes

Full document available:
Yes — 141 pages

Real organization:
Yes

Real customer data:
Yes

Organizational diagnosis:
Yes

Multiple analytical approaches:
Yes

Implementation plan:
Yes

Production considerations:
Yes

Long-term production ROI demonstrated:
No

---

## Key Product Principle

Do not stop at understanding how the customer feels.

Understand what happened, determine how important it is, and connect the
customer signal to the business action that should happen next.

---

## Status

Research completed
