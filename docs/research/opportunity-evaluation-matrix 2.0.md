# Gintech Product Lab — Opportunity Evaluation Matrix

## Purpose

Compare opportunity areas and concrete customer segments to determine where Gintech should begin product discovery.

This document updates Version 1 using the twelve reference cases. It separates external evidence, Gintech interpretations and assumptions requiring validation.

The matrix supports a discovery decision. It does not establish customer demand, product-market fit or MVP scope.

## Status

- **Version:** 2.0
- **Updated:** October 3, 2026
- **Stage:** Segment Comparison and Validation Planning
- **Research Foundation:** Cases 01–12
- **Decision Status:** B2B distributors proposed; initial segment not yet formally adopted
- **Customer and Data Validation:** Pending
- **Related Issue:** [#1 — Initial target segment](https://github.com/ramanjarres/gintech-product-lab/issues/1)

---

## 1. Changes from Version 1

| Previous approach | Version 2 treatment |
|---|---|
| Four reference cases | Twelve reference cases |
| Intelligence areas treated as candidate segments | Solution areas and customer segments evaluated separately |
| Assumed access and data availability assigned scores | Unknowns explicitly marked Pending |
| Weighted ranking drove the initial interpretation | Qualitative comparison guides the next evidence collection |
| Industrial entry barriers centered on telemetry | Existing maintenance records remain a possible path |
| Technical feasibility emphasized | Customer access, decision ownership and value measurement included as conditions |

The previous scores remain part of the Git history. They are not the current market ranking.

### Historical calculation correction

Applying Version 1's weights to its original ratings gives:

| Opportunity area | Published score | Correct calculation |
|---|---:|---:|
| Customer Intelligence | 4.65 | 4.70 |
| Operations Intelligence | 4.20 | 4.20 |
| Demand Intelligence | 4.15 | 4.20 |
| Industrial Intelligence | 2.70 | 2.85 |

These corrections do not validate the underlying ratings. In particular, public data availability is not proof of access to buyers or customer-owned records.

---

## 2. Research Foundation

| # | Case | Contribution to this comparison |
|---|---|---|
| 01 | Airbnb | Customer intent and interaction handling |
| 02 | Ricoh | Service resolution and dispatch decisions |
| 03 | Nestlé | Demand and planning |
| 04 | SENER | Equipment anomaly detection |
| 05 | AI4Time | Maintenance history and asset prioritization |
| 06 | Megatiendas | Store demand and inventory planning |
| 07 | Vanti | Customer feedback and issue identification |
| 08 | Héctor Ocaña | Demand, capacity and logistics planning |
| 09 | Crece Más | Traditional-channel digitalization |
| 10 | TrackApp — research pseudonym | Analytics informing product adaptation |
| 11 | Maderkit | Reporting integration and information access |
| 12 | Alico | Reported inventory improvement and specialized production planning |

Cases 01–08 are carried forward from the existing case documentation and synthesis. Cases 09–12 add context but do not resolve all original research questions.

### Evidence limitations of the final cycle

- **Crece Más:** Product and implementation descriptions; business outcomes reported by AWS without a public measurement methodology.
- **TrackApp:** Academic qualitative case; an analytics-oriented startup in Greece, using a confidentiality pseudonym. Transferability to typical local SMEs remains uncertain.
- **Maderkit:** Provider description of SIESA integration, Power BI, SQL Server and self-service reporting. This is not a formal data-quality audit.
- **Alico:** TCP reports a 50% inventory reduction using a statistical model based on 18 months of ERP information. The public material does not establish an independently verified ROI calculation.

External cases remain Level 2 — Secondary Evidence for Gintech. They do not establish direct customer, data or commercial evidence for its proposed offer.

---

## 3. Working Business Pattern

Business problem → Available data → Analysis → Business context → Decision → Action → Outcome measurement.

This is a working interpretation across the research. Not every case documents every step.

For a future pilot, Gintech must identify the decision owner, available alternatives, operational constraints and outcome before selecting a technical method.

---

## 4. Opportunity Areas

These categories describe capabilities, not customer segments.

| Area | Potential decision | Potential inputs | Main uncertainty |
|---|---|---|---|
| Customer Intelligence | Which recurring customer problem needs attention? | Messages, PQRS, tickets and surveys | Differentiation and connection to action |
| Operations Intelligence | How should resources or work be prioritized? | Incidents, orders, capacity and operational events | Repeatability across processes |
| Demand Intelligence | What inventory requires replenishment attention? | Sales, stock, purchases and lead times | Record reliability and purchasing constraints |
| Industrial Intelligence | Which asset needs attention and when? | Maintenance records, inspections and telemetry | Domain expertise, usable history and implementation risk |

### Revised interpretation

- Customer Intelligence remains a plausible direction, particularly where Gintech can connect issues to measurable operational responses.
- Operations Intelligence requires a narrow decision; the broad category is insufficient for product selection.
- Demand Intelligence offers a testable inventory direction when usable records and a decision owner are available.
- Industrial Intelligence is not excluded solely because new sensors might be required. Existing records may support some use cases, subject to inspection.

These are hypotheses, not measured statements about the Colombian market.

---

## 5. Evaluation Criteria

The original criteria are retained. Their weights remain provisional and are not used to generate a Version 2 total.

| Criterion | Legacy weight | Question | Evidence needed |
|---|---:|---|---|
| Problem frequency | 10% | How often is the decision made or the problem experienced? | Specific recent examples and process records |
| Business impact | 15% | What happens when the decision is poor or delayed? | Baseline costs, service outcomes or operational consequences |
| Data availability | 15% | Are necessary records captured and fit for this use? | Authorized anonymized samples and coverage checks |
| Access to customers | 15% | Can Gintech reach decision-makers? | Named prospects and scheduled conversations |
| MVP feasibility | 15% | Can one useful decision be tested within a limited scope? | Agreed workflow, integration constraints and effort estimate |
| Time to value | 10% | When could a meaningful outcome be observed? | Decision cycle and measurement window |
| Technical complexity | 5% | What expertise, dependencies and maintenance are needed? | Data and process inspection |
| Validation with real data | 10% | Will a customer permit a decision-relevant test? | Authorized data access and a suitable sample |
| Willingness to pay | 5% | Who has budget and what commitment would they make? | Current spending, purchasing process and commercial behavior |
| **Total legacy weights** | **100%** | | |

Synthetic or public data can test implementation, but cannot by itself validate a specific customer's problem or economic value.

### Assessment labels

- **External evidence:** Supported by a reviewed external case; transferability remains untested.
- **Hypothesis:** A Gintech judgment requiring investigation.
- **Pending:** Insufficient direct evidence to assess.
- **Customer-confirmed:** Supported by a recorded customer account, limited to that context.
- **Data-tested:** Examined quantitatively using authorized customer records.

Do not substitute a neutral numerical score for missing evidence. Confidence and attractiveness must be documented separately.

---

## 6. Candidate Customer Segments

The following definitions are discovery candidates, not established customer profiles. Geography is a proposed scope.

| Segment | Proposed discovery boundary | Participant | Decision to investigate |
|---|---|---|---|
| Customer support operations | Organizations serving customers in Colombia with structured ticket or complaint records | Support or customer-experience manager | Which recurring issue should be prioritized for corrective action? |
| Retail businesses | Local retailers with recorded sales, purchases and stock | Owner, purchasing or inventory manager | Which products require replenishment attention? |
| Restaurants and food businesses | Local businesses with recorded sales, stock and waste | Owner or operations manager | Which ingredients require purchasing attention before the next cycle? |
| B2B distributors | Small and medium-sized distributors in Barranquilla and Atlántico with structured operational records | Owner, purchasing or operations manager | Which products require replenishment attention before the next purchasing cycle? |
| Industrial manufacturers | Regional manufacturers with accessible maintenance history | Maintenance or operations manager | Which assets require maintenance attention first? |

Restaurants are evaluated separately because their operational requirements should not be assumed equivalent to retail. Service businesses remain a broad backlog category until a concrete recurring decision is specified.

---

## 7. Qualitative Segment Comparison

| Segment | External evidence and its limits | Gintech capability fit — interpretation | Proposed pilot and principal risk |
|---|---|---|---|
| Customer support | Airbnb, Ricoh and Vanti provide related patterns; enterprise cases do not establish local buyer access | Closest to Rafael's experience in issue analysis, prioritization and operational reporting | Prioritize one recurring issue using authorized records; recommendations may lack an owner able to act |
| Retail | Megatiendas and Crece Más provide related context; stores and implementations differ | Operational and inventory analysis would require customer-specific learning | Review replenishment exceptions for a limited assortment; stock accuracy and adoption may be obstacles |
| Restaurants and food | No dedicated restaurant case in this cycle; retail evidence is indirect | Requires investigation of recipes, purchasing, stock and waste | Test one ingredient-purchasing workflow; preparation and yield records may be insufficient |
| B2B distributors | Demand and logistics cases provide adjacent evidence; repeatability in local distributors is unverified | Combines operational analysis and a concrete inventory decision, with domain learning required | Review replenishment exceptions for one product category; supplier constraints and integration may dominate |
| Industrial manufacturers | SENER and AI4Time provide relevant maintenance patterns; Alico adds planning context | Domain knowledge and engineering support may be needed | Review maintenance priorities for a limited asset group; failure history may not support reliable analysis |

### Direct evidence still required

| Segment | Customer access | Usable customer data | Problem cost and frequency | Budget and payment evidence |
|---|---|---|---|---|
| Customer support | Pending | Pending | Pending | Pending |
| Retail | Pending | Pending | Pending | Pending |
| Restaurants and food | Pending | Pending | Pending | Pending |
| B2B distributors | Pending | Pending | Pending | Pending |
| Industrial manufacturers | Pending | Pending | Pending | Pending |

This table is intentionally not a market ranking. The case studies do not resolve these unknowns.

Professional experience does not establish permission to use employer records or access to external buyers.

---

## 8. Proposed Direction and Alternative

### Current proposal: B2B distributors

Explore small and medium-sized B2B distributors in Barranquilla and Atlántico that already maintain structured sales, inventory and purchasing records.

Investigate one decision:

> Which products require replenishment attention before the next purchasing cycle?

This is a focused and potentially measurable discovery hypothesis. It is not established as superior to the alternatives.

### Active comparison: Customer support operations

Retain customer support as an active comparison because it has the closest documented alignment with Rafael's experience.

Investigate:

> Which recurring customer issue should be prioritized for corrective action?

Customer access and implementation feasibility may justify choosing this direction instead. They must be investigated rather than inferred from professional familiarity.

### Decision status

No final initial segment is adopted in this document. B2B distributors remain the proposal recorded in the synthesis and issue update.

Retail, restaurants and industrial maintenance remain alternatives. None is permanently rejected by this preliminary comparison.

---

## 9. Selection Conditions

A discovery segment may be adopted before the problem is commercially validated. It needs a realistic research path.

Before adoption, document:

1. Specific prospects and a feasible route to conversations.
2. The participant responsible for the candidate decision.
3. Reasons for prioritizing this segment over the alternatives.
4. Unknowns and evidence that would change the selection.
5. The connection to the problem statement and business context.

Before proposing a data pilot, verify:

- A repeated problem that is insufficiently addressed today.
- Authorized access to records suitable for the decision.
- Feasible actions under the customer's constraints.
- An observable baseline and outcome.
- A customer willing to invest time and participate.
- Delivery effort proportionate to potential value.

Commercial viability requires further evidence about budget, payment, acquisition, maintenance and repeatability.

---

## 10. Risks and Assumptions

| Assumption or risk | Investigation | Consequence if unsupported |
|---|---|---|
| Local presence will make distributors accessible | Identify contacts and attempt interview scheduling | Reconsider the discovery segment |
| Operational records are usable | Inspect authorized samples, coverage and definitions | Address specific gaps or stop the proposed pilot |
| Stockouts hide unmet demand | Compare sales with availability records | Avoid treating sales as unconstrained demand |
| Better information changes a decision | Examine recent decisions and feasible alternatives | Reframe or reject the problem |
| The customer can act on a recommendation | Identify owner, approval process and constraints | Revise delivery or choose another decision |
| The decision repeats across firms | Compare independent customer workflows | Limit customization or treat the work as a service |
| Value exceeds delivery cost | Estimate and subsequently measure both | Do not pursue the implementation solely to generate revenue |
| The user is also the buyer | Investigate budget ownership and procurement | Adapt the commercial hypothesis |
| Lower stock is beneficial | Measure availability and fulfillment alongside stock | Avoid improving inventory at the expense of service |

---

## 11. Evidence Collection Plan

### Immediate comparison

1. Identify potential interview participants in B2B distribution and customer support.
2. Record actual access, rather than assumed accessibility.
3. Ask for recent examples of the candidate decision, its current process and consequences.
4. Investigate existing tools, spending and satisfaction with current workarounds.
5. Request an authorized anonymized sample only where a data diagnostic is justified.
6. Update this matrix using the resulting evidence.

The first interviews guide research. They are not a representative market estimate.

### Evidence record

For each finding, record:

- Source or interview identifier
- Date and business context
- Specific claim
- Evidence type
- Criterion affected
- Supporting record, where available
- Limitations or contradictory evidence
- Implication for the proposed segment

Keep identifying or sensitive customer information out of the public repository.

---

## 12. Future Scoring Rule

Numerical scoring may be reintroduced when criteria have explicit, comparable anchors and adequate evidence.

Requirements:

- Define what each score means for each criterion.
- Record the evidence supporting each rating.
- Keep unknowns unscored; do not treat Pending as zero or three.
- Avoid comparing partial totals with different evidence coverage.
- Review overlap between data availability and validation access.
- Review overlap between feasibility, complexity and time to value.
- Reconsider the legacy 5% payment weight when evaluating commercial viability.
- Treat customer access and pilot feasibility as conditions that a high total cannot override.

This version has no updated weighted winner.

---

## 13. Relationship to Issue #1

| Acceptance criterion | Current position |
|---|---|
| At least three segments compared | Addressed by this document |
| Selection criteria documented | Addressed by this document |
| One initial segment selected | Pending formal adoption |
| Risks and assumptions documented | Addressed by this document |
| Decision linked to problem statement and business context | Pending actual repository links and updates |

Keep issue #1 open and In Progress until the adopted decision and supporting document links are recorded.

Closing the selection issue would document a discovery decision. It would not mean that the problem or market has been validated.

---

## 14. Next Action

Compare practical interview access for B2B distributors and customer support operations, then adopt and document one initial discovery segment.

Update the problem statement and business context around the selected decision. Customer discovery and data inspection should precede requirements, dashboard design and MVP implementation.

## References

The existing case-study documents and Research Synthesis 01–12 provide the research foundation. Add their actual repository links when committing this file; unverified filenames are not assumed here.

Additional external sources for the final research cycle:

- [Crece Más — official product website](https://www.crecemas.com/)
- [PUCP — Crece Más project description](https://investigacion.pucp.edu.pe/noticias-y-eventos/crece-mas-solucion-tecnologica-para-las-mypes/)
- [AWS — Crece Más case study](https://aws.amazon.com/jp/solutions/case-studies/crece-mas-facele/)
- [Zamani, Griva and Conboy (2022) — TrackApp study](https://doi.org/10.1007/s10796-022-10255-8)
- [CepoBIA — Maderkit case study](https://www.cepobia.com/caso-de-exito-maderkit/)
- [TCP — Alico case study](https://www.tcpamericas.com/es/case-studies/Alico-data-driven-growth)

Provider-reported outcomes are not independently verified market evidence for Gintech.
