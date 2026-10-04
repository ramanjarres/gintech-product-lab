# Case Study: Airbnb Message Intent Classification

## Source
Company: Airbnb
Year: 2019
Domain: Customer Intelligence / NLP
Source: Discovering and Classifying In-app Message Intent at Airbnb

## Business Problem
Airbnb needed to understand the intent behind large volumes of
messages exchanged between guests and hosts.

## Data
Unstructured conversational text from in-app messages.

## Approach
1. Topic discovery using unsupervised learning (LDA)
2. Human validation and taxonomy creation
3. Manual labeling
4. Supervised intent classification using CNN
5. Production deployment

## Key Findings
- Customer messages can contain multiple intents.
- Taxonomy quality strongly affects classification performance.
- Human validation remains important.
- Airbnb achieved approximately 70% overall classification accuracy.
- Understanding intent can enable earlier intervention.

## Business Applications
- Identify customer support issues
- Detect cancellation, payment and refund intents
- Understand customer concerns
- Enable smarter responses

## Limitations / Lessons
- Label ambiguity affects model accuracy.
- Human labeling can introduce errors.
- Multi-intent messages require special handling.
- The 2019 technical architecture should not automatically be
  considered the best architecture today.

## Gintech Relevance
This case supports the hypothesis that Gintech could transform
unstructured customer feedback into structured business intelligence.

Potential inputs:
- Surveys
- Reviews
- Support tickets
- Chats
- Call transcripts

Potential outputs:
- Intent
- Topic
- Sentiment
- Severity
- Frequency
- Emerging issues
- Recommended actions

## Product Hypothesis
Can Gintech automatically discover, classify and prioritize customer
problems from unstructured feedback and translate them into
recommended business actions?

## Related Gintech Capability
Customer Intelligence

## Status
Research completed
