# Case Study 11 — Maderkit

## Research Metadata

- **Organization:** Maderkit
- **Region:** Colombia
- **Industry:** Furniture manufacturing and sales
- **Implementation Provider:** CepoBIA
- **Research Focus:** Data integration, reporting readiness and access
- **Evidence Type:** Implementation-provider case study
- **Research Status:** Secondary research documented

---

## 1. Research Question

When business data already exists, what prevents it from becoming
reliable and accessible information for a recurring decision?

---

## 2. Documented Business Problem

According to CepoBIA, financial staff manually assembled monthly
income statements and balance sheets in Excel using SIESA data.

Commercial reports covering inventory, sell-out, freight, sales
and average ticket existed in separate spreadsheets.

Users depended on area leaders to obtain reports.

Source: [1]

---

## 3. Documented Approach

The provider reports:

- Direct extraction from SIESA
- Power BI and SQL Server
- A shared, governed information source
- A self-service portal for authorized users

Source: [1]

---

## 4. Reported Results

| Dimension | Reported change |
|---|---|
| Preparation | Previously one or two days of manual report assembly |
| Availability | Information described as available in near real time |
| Frequency | Monthly reporting replaced by daily access |
| Access | Authorized users could consult reports directly |
| Governance | A common source replaced separate departmental versions |

Source: [1]

---

## 5. Evidence Boundaries

The publication does not disclose:

- A formal data-quality assessment
- Refresh-latency measurements
- Implementation costs or quantified ROI
- Specific decisions and their measured outcomes

Manual preparation time and refresh latency are different measures.
They should not be converted into a percentage improvement.

The provider's governance description does not independently verify
data accuracy.

For Gintech, this remains Level 2 — Secondary Evidence.

---

## 6. Gintech Interpretation

### Existing data is only the starting point

Gintech should investigate whether information is usable for the
specific decision under study.

Data may exist but still require work on access, interpretation,
integration or reliability.

### Information access is an intermediate outcome

A proposed Gintech pilot should distinguish:

1. Information became accessible.
2. The responsible person used it.
3. The information changed a decision.
4. The resulting action improved an agreed business outcome.

Each stage requires its own evidence.

### Data readiness and data quality are related but distinct

For Gintech:

- **Data quality** concerns whether records are fit for the intended use.
- **Data readiness** also includes access, history, definitions,
  integration, refresh frequency and operational ownership.

A readiness assessment should be scoped to one decision rather than
trying to certify an entire organization.

---

## 7. Proposed Data Readiness Assessment

This framework is a Gintech proposal, not a documented Maderkit method.

| Dimension | Diagnostic question | Evidence to request |
|---|---|---|
| Availability | Are the required records captured? | Anonymized sample |
| Access | Can authorized staff retrieve them? | Export or integration process |
| Completeness | Are essential fields missing? | Missing-value profile |
| Consistency | Do sources use compatible definitions? | Data dictionary and reconciliation |
| Timeliness | Is information current enough to act? | Transaction and refresh timestamps |
| History | Is there enough history for the proposed analysis? | Coverage by period |
| Ownership | Who resolves discrepancies? | Named business and technical owners |
| Decision fit | Would better information change an action? | Current decision workflow |

The outcome should be an explicit recommendation:

- Proceed with a limited pilot
- Resolve specific readiness gaps first
- Stop because the proposed use case lacks sufficient value or feasibility

---

## 8. Potential Decision Points

The following are hypotheses for customer discovery, not outcomes
documented in the case.

| Potential decision | Information required | Possible action |
|---|---|---|
| Which inventory needs attention? | Stock, sales and movement history | Review replenishment or allocation |
| Which customer relationship needs review? | Revenue and attributable costs | Investigate profitability |
| Which freight expense needs investigation? | Cost by shipment and route | Review operational causes |

Before selecting a pilot, identify the decision owner, constraints,
frequency and cost of a poor decision.

---

## 9. Product Hypothesis

> Organizations with fragmented reporting may benefit from a
> focused diagnostic that identifies the data gaps preventing
> one valuable business decision from improving.

This could become an entry service for Gintech.

It is not yet evidence that customers will pay for a standalone
data-readiness product.

---

## 10. Proposed Validation

1. Select one recurring decision with a potential customer.
2. Map the current reporting and decision process.
3. Measure preparation effort and information delay separately.
4. Inspect public, synthetic or anonymized sample data.
5. Identify the minimum changes needed for a pilot.
6. Agree on the decision owner and target outcome.
7. Test whether improved information changes an action.
8. Compare the outcome against an agreed baseline.
9. Evaluate implementation and maintenance costs.
10. Decide whether to continue, revise or stop.

---

## 11. Research Gaps

- Is the problem frequent across accessible target companies?
- What do they currently spend on reporting?
- Which reporting delays actually affect decisions?
- Who controls the budget and source-system access?
- Would they pay for diagnosis separately from implementation?
- Can the work be repeated without extensive customization?
- What support is required after deployment?
- How can Gintech demonstrate value beyond faster report production?

---

## 12. Research Conclusion

For Gintech, this case motivates investigating the work required
between existing business records and usable decision information.

The next step is to test a narrowly scoped readiness assessment
with potential customers.

A successful diagnostic must identify a feasible decision
improvement and its measurement plan.

---

## Source

[1] CepoBIA.
“Caso de éxito Maderkit.”
Published July 1, 2026.

https://www.cepobia.com/caso-de-exito-maderkit/

Evidence classification:
Provider-reported implementation; independent validation remains pending.
