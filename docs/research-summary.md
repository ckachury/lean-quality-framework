# Research summary

## Method

- **Model:** TMMi, used as a self-assessment questionnaire scored 1 to 5 by maturity level and process area.
- **Sample:** 10 Chilean tech startups across four stages: pre-seed, seed, growth and IPO / consolidation.
- **Respondents:** 70% in management or C-level roles. 70% of startups had teams of five developers or fewer; 50% were in growth stage.
- **Complement:** interviews with founders and technical leaders to understand the reasons behind the scores.

Results are aggregated. No company is identified.

## Main findings

1. **Maturity between levels 2 and 3.** 70% of startups sit at level 2 (Managed) or 3 (Defined): processes exist but are not standardised.
2. **Measurement and improvement are the gaps.** Levels 4 and 5 average 2.8; decisions rely on intuition more than data.
3. **Defect management is the strength (4.1)**, followed by test planning. Roles and responsibilities, metrics and continuous improvement are weakest.
4. **Quality is reactive.** 50% focus on catching errors or "keeping things from blowing up"; 30% work on systematic prevention.

## Average score by stage (1 to 5)

| Stage | Level 2 · Managed | Level 3 · Defined | Level 4 · Measured | Level 5 · Optimization |
|---|---|---|---|---|
| Pre-seed | 4.00 | 3.00 | 2.50 | 1.50 |
| Seed | 3.50 | 3.12 | 2.00 | 4.00 |
| Growth | 3.75 | 3.50 | 3.00 | 2.40 |
| IPO / consolidation | 4.75 | 5.00 | 4.00 | 5.00 |

Small groups per stage: read the table as patterns, not as statistically representative values.

## From gaps to framework components

| Stage | Gap (data) | LQF-S component | Type of service |
|---|---|---|---|
| Pre-seed | No continuous improvement (level 5 = 1.5) | Lean quality foundations | Diagnosis and quick wins |
| Pre-seed | Weak test organisation (level 3 = 2.0) | Minimum QA organisation | Lightweight process design |
| Seed | No quality metrics (level 4 = 2.0) | Essential risk-based metrics | Focused implementation |
| Seed | Unclear QA roles (level 3 = 2.5) | Roles and ownership | Organisational design |
| Growth | Reactive improvement (level 5 = 2.4) | Improvement and feedback loops | Optimisation project |
| Growth | QA integrated but not systematic (level 3 ≈ 3.0) | QA–Dev–Business integration | Incremental implementation |
| IPO | Need for standards and benchmarks | Scaling and quality governance | Advanced consulting |

## Recommendations

- **Roles:** name a QA owner per squad and formalise Definition of Ready and Definition of Done.
- **Metrics (GQM):** a basic dashboard with defects by severity, lead and flow time, minimum coverage and rework percentage.
- **Infrastructure:** isolated staging environments and basic quality gates in CI/CD.
- **Quick wins in 4 to 8 weeks:** acceptance criteria on every story, a smoke and regression set per release, a standard bug report template, a TMMi baseline to measure progress.
