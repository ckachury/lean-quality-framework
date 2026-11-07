# LQF-S in detail

## 1. Business-driven quality goals (GQM)

Instead of chasing abstract technical targets such as 100% code coverage, quality goals are tied to business goals with an adaptation of Goal-Question-Metric.

| Level | Question it answers | Example |
|---|---|---|
| Goal | What does the startup want to achieve? | Increase first-month retention of new users by 15% |
| Question | What do we need to know about product quality to reach it? | Are bugs in onboarding frustrating new users and making them leave? |
| Metric | How do we measure the answer simply? | Critical errors reported by users in their first 24 hours; drop-off rate in the onboarding funnel |

Rules of thumb:

- One to three goals per quarter. More goals means no focus.
- Every metric must be able to change a decision. If nobody would act on it, drop it.
- Review the metrics in the sprint retrospective.

Template: [gqm-canvas.md](../templates/gqm-canvas.md).

## 2. Risk-first matrix

Startups cannot fix everything. The matrix shows where quality effort pays off.

- **Business impact (vertical):** how serious would a failure be? Low, medium, high, critical. Impact can be financial, reputational or legal.
- **Likelihood of failure (horizontal):** how likely is it to fail? Low, medium, high. Based on technical complexity, lack of tests, recent changes.
- Map the product's key features. Those in **high impact / high likelihood** get the most attention: more tests, code review, monitoring.

Template: [risk-matrix.md](../templates/risk-matrix.md).

## 3. Agile quality loop

Quality practices become part of the sprint and of the Definition of Done.

| Step | When | Practice |
|---|---|---|
| Plan | Sprint planning | For prioritised stories, especially high-risk ones, define quality criteria beyond functional acceptance: performance, security, usability. *Example: payment completes in under 3 seconds in Chrome, Safari and Firefox.* |
| Do | During the sprint | Practices scaled by risk (below) |
| Verify | Retro and next planning | Production monitoring, user feedback (support tickets, reviews), GQM metrics |

Practices by risk:

| Risk | Practices |
|---|---|
| Low | Exploratory testing by the developer |
| Medium | Peer code review, key unit tests |
| High / critical | Automated end-to-end tests, basic security testing, usability testing with real users |

## 4. Evolving maturity roadmap

Quality maturity grows with business maturity.

| Phase | Focus | Practices to introduce |
|---|---|---|
| MVP / validation (up to ~500 users) | Speed and feedback. Quality means "don't break catastrophically" | Exploratory manual testing, basic risk matrix, production error monitoring |
| Growth / product-market fit (~500 to 10,000 users) | Stabilise and retain. Reliability and user experience | Automation of critical happy paths, systematic code review, performance metrics |
| Scale (10,000+ users) | Efficiency and robustness for sustainable growth | Load and stress testing, mature CI/CD, defined quality roles |

User counts are orientation, not rules. Move to the next phase when the signals of the current one appear: incidents that cost customers, slower releases because of fear, or investors asking about reliability.
