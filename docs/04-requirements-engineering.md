# Requirements Engineering

## Purpose

This document explains how requirements engineering will be applied to Gintech Product Lab.

The goal is to make sure the project does not start by building features without first understanding the business problem, user needs, constraints, and expected outcomes.

## What Is Requirements Engineering?

Requirements engineering is the process of discovering, analyzing, documenting, validating, and managing the needs that a software system must satisfy.

For this project, requirements engineering will help answer:

- What problem are we solving?
- Who has the problem?
- What does the user need?
- What should the system do?
- What constraints must the system respect?
- How will we know if the requirement was successfully met?
- How will changes to requirements be managed?

## Why It Matters

A software product can be technically correct but still fail if it does not solve the real user or business problem.

Requirements engineering reduces this risk by helping the team:

- Understand customer and business needs.
- Define the scope of the product.
- Avoid ambiguous requirements.
- Prioritize what should be built first.
- Validate requirements before development.
- Create clear acceptance criteria.
- Maintain traceability between problems, requirements, features, and tests.

## Requirements Engineering Stages

### 1. Elicitation

Elicitation is the process of discovering needs from users, stakeholders, business context, and available data.

Possible elicitation methods for this project:

- Interviews with business owners.
- Surveys.
- Observation of business processes.
- Analysis of customer feedback.
- Review of operational reports.
- Study of existing tools and competitors.
- Analysis of public or synthetic datasets.

Example questions:

- What information do you collect today?
- Where is that information stored?
- What problems are repeated frequently?
- How do you decide what to improve first?
- What decisions are difficult to make with your current data?
- How do you know if an improvement worked?

---

### 2. Analysis

Analysis is used to review the information collected during elicitation and identify conflicts, gaps, ambiguities, and priorities.

For this project, analysis will focus on:

- Identifying repeated business problems.
- Understanding user pain points.
- Detecting unclear or conflicting needs.
- Grouping requirements by theme.
- Evaluating feasibility.
- Connecting requirements with business value.
- Prioritizing what should be part of the MVP.

Example:

A user may say:

> “I need to know what customers are complaining about.”

This must be analyzed and converted into clearer requirements, such as:

- The system should allow customer feedback to be categorized by topic.
- The system should show the most frequent complaint categories.
- The system should allow filtering feedback by date, source, or business area.

---

### 3. Specification

Specification is the documentation of requirements in a clear and structured way.

For this project, requirements may be documented as:

- Functional requirements.
- Non-functional requirements.
- User stories.
- Acceptance criteria.
- Use cases.
- Process flows.
- Data requirements.
- Business rules.

Example user story:

> As a business owner, I want to see the most frequent customer complaints so that I can decide which problem to address first.

Example acceptance criteria:

- The system displays complaint categories ranked by frequency.
- The user can filter results by date range.
- The user can see the number of complaints per category.
- The information updates when new data is added.

---

### 4. Validation

Validation ensures that the documented requirements actually match user and business needs.

Validation methods may include:

- Reviewing requirements with potential users.
- Creating wireframes or prototypes.
- Testing assumptions with surveys or interviews.
- Comparing requirements with real business scenarios.
- Using sample data to check whether the requirement is useful.
- Defining measurable acceptance criteria.

The goal is to avoid building a technically correct solution that does not create real value.

---

### 5. Requirements Management

Requirements may change as the project evolves.

This project will manage changes by documenting:

- Original requirement.
- Reason for change.
- Impact on scope.
- Impact on data or design.
- Priority.
- Status.
- Related user story or feature.

## Types of Requirements

### Functional Requirements

Functional requirements describe what the system should do.

Examples:

- The system should allow users to upload customer feedback data.
- The system should categorize feedback by topic.
- The system should display issue frequency.
- The system should calculate an impact score.
- The system should allow users to filter results by date, source, or category.

### Non-Functional Requirements

Non-functional requirements describe quality attributes, constraints, or performance expectations.

Examples:

- The dashboard should load in less than 3 seconds for standard datasets.
- The interface should be simple enough for non-technical users.
- The system should protect sensitive customer information.
- The system should be usable from a web browser.
- The data model should support future AI/ML experimentation.

## Characteristics of Good Requirements

A good requirement should be:

- Clear
- Necessary
- Complete
- Consistent
- Feasible
- Prioritized
- Verifiable
- Traceable
- Modifiable

## Initial Requirement Template

Each requirement should be documented using the following structure:
Requirement ID: FR-001
Requirement type: Functional
Description: The system should allow users to upload customer feedback data from a CSV file.
User need: Business users need to analyze customer feedback collected from different sources.
Business value: Enables structured analysis of customer problems.
Priority: High
Acceptance criteria:
- User can upload a CSV file.
- System validates required columns.
- System shows an error if the file format is invalid.
- Uploaded data becomes available for analysis.
Source: Initial product hypothesis
Status: Draft
Related feature: Data upload
Related user story: As a business user, I want to upload customer feedback data so that I can analyze recurring problems.

```text
Requirement ID:
Requirement type:
Description:
User need:
Business value:
Priority:
Acceptance criteria:
Source:
Status:
Related feature:
Related user story:
