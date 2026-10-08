# Management Review

> **Simulated portfolio project.** SecurePay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

| | |
|---|---|
| **Document ID** | SP-ISMS-MRV-001 |
| **Meeting date** | October 2026 (simulated) |
| **Chair** | CEO |
| **Attendees** | CTO, Security Lead, IT Manager, DevOps Lead, HR Manager, Finance Manager |
| **Standard** | ISO/IEC 27001:2022 clause 9.3 |

## 1. Inputs reviewed
- Status of actions from previous reviews: none (first review).
- Changes in internal/external issues and interested parties' requirements.
- Information security performance (KPIs below), audit results and non-conformities.
- Risk assessment results and treatment plan status.
- Opportunities for continual improvement.

## 2. KPIs (fictional)
| KPI | Value | Target | Status |
|---|---|---|---|
| MFA Coverage | 82% | 100% | Red |
| Security Training Completion | 94% | 95% | Amber |
| Open Critical Risks | 1 | 0 | Red |
| Open High Risks | 17 | <=5 | Red |
| Critical Vulnerabilities >30 days | 2 | 0 | Red |
| Access Reviews Completed | 75% | 100% | Amber |
| Incident Response SLA | 91% | 95% | Amber |
| Backup Restore Tests Completed | 0 | 4 per year | Red |

*Note: the brief listed 8 open High risks; the register contains 17 High and 1 Critical (18 total), so the review uses the register figures. Targets are portfolio assumptions.*

## 3. Audit and risk summary
- Internal audit: 3 Pass, 3 Partial, 1 Fail from the checklist (see `07-Internal-Audit/`); 4 findings (2 Major, 2 Minor).
- Risks: 1 Critical (R-001), 17 High. Projected residual after treatment: all at or below Medium (see Risk Register).

## 4. Management decisions
| # | Decision | Owner | Deadline |
|---|---|---|---|
| 1 | Achieve 100% MFA coverage | IT Manager | 30 days |
| 2 | Complete quarterly privileged-access reviews | CTO | Quarterly |
| 3 | Conduct backup restoration testing | DevOps Lead | 30 days |
| 4 | Establish formal vendor security assessments | Procurement | 60 days |
| 5 | Perform annual security-awareness training | HR / Security Lead | Annual |

## 5. Outputs
- Resources approved for EDR rollout, secret management and DR design.
- ISMS scope, policy and objectives confirmed as suitable.
- Next management review: within 12 months, or earlier after a major incident.

## 6. Continual improvement
Corrective actions are tracked in `08-Corrective-Actions/Corrective-Action-Plan.xlsx` and re-tested at the next internal audit, closing the loop: risk -> treatment -> control -> evidence -> audit -> management review.
