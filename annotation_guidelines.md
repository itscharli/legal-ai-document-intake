# Legal Document Annotation Guidelines

**Version:** 1.1
**Dataset:** Synthetic legal operations documents
**Status:** Initial annotation protocol

## Objective

Establish consistent labeling rules for classifying incoming legal documents according to their primary purpose.

## Classification Labels

| Label | Definition |
|---|---|
| NDA | A standalone agreement primarily establishing confidentiality or nondisclosure obligations. |
| EMPLOYMENT_AGREEMENT | An agreement primarily establishing employment terms, compensation, responsibilities, or termination provisions. |
| COURT_DOCUMENT | A filing, order, judgment, or other record associated with formal court proceedings. |
| NEEDS_REVIEW | A document that is incomplete, ambiguous, outside the supported categories, or insufficiently clear to classify. |
| GOVERNMENT_AGENCY_OPINION | A formal written opinion or interpretation issued by a government administrative agency in response to a legal or regulatory question.|

## Annotation Rules

1. Read the entire available document before assigning a label.
2. Determine its primary purpose rather than relying solely on keywords or titles.
3. Consider supporting clauses and contextual evidence.
4. Do not classify an employment agreement as an NDA solely because it contains a confidentiality provision.
5. Use NEEDS_REVIEW when the available evidence does not support a reliable classification.
6. Record a confidence level: High, Medium, or Low.
7. Document the evidence supporting each classification decision.
8. Do not invent missing information.

## Confidence Definitions

- High: Clear evidence supports one category with no material ambiguity.
- Medium: The most likely category is identifiable, but uncertainty remains.
- Low: Evidence is weak or contradictory; consider NEEDS_REVIEW.

## Human Review

Documents with ambiguous or conflicting purposes, missing critical information, or classifications outside the supported categories should be routed for human review.

## Data Privacy

Use only fictional, synthetic, or appropriately licensed documents. Never upload confidential legal or client records.

## Limitations

These guidelines are an introductory document annotation framework, not legal advice or a substitute for professional legal review. Confidence levels reflect annotator judgment rather than calibrated model probabilities.
