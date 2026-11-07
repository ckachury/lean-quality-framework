# Risk-first matrix

## Run it in one hour

1. **List features (10 min).** Product, tech lead and QA list the 10 to 20 features or flows that matter most.
2. **Rate impact (15 min).** For each: if it fails, what happens to the business? Low, medium, high, critical.
3. **Rate likelihood (15 min).** How likely is it to fail? Consider complexity, recent changes, test coverage and incident history.
4. **Place and agree (10 min).** Put each feature in the grid. Discuss only the disagreements.
5. **Decide (10 min).** For the top-right cells, agree the quality practices for the next sprint.

## Grid

|  | Low likelihood | Medium likelihood | High likelihood |
|---|---|---|---|
| **Critical impact** | Monitor | Prioritise | **Act now** |
| **High impact** | Monitor | Prioritise | Prioritise |
| **Medium impact** | Accept | Monitor | Prioritise |
| **Low impact** | Accept | Accept | Monitor |

## What each zone means

| Zone | Quality effort |
|---|---|
| Act now | Automated end-to-end tests, code review, monitoring and alerting, security checks |
| Prioritise | Key unit and integration tests, peer review, exploratory sessions before release |
| Monitor | Production error monitoring and user feedback |
| Accept | Developer exploratory testing; fix when found |

Re-run the matrix every quarter, or when a major feature, a new market or an incident changes the picture.
