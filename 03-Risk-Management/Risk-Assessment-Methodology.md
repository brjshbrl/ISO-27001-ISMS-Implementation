# Risk Assessment Methodology

> **Simulated portfolio project.** HawkPay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

**Document ID:** HP-ISMS-MTH-001 | **Version:** 1.0 | **Owner:** Security Lead | **Date:** October 2026

## 1. Approach
Asset-based and threat/vulnerability-driven (ISO/IEC 27001:2022 clause 6.1.2, guided by ISO/IEC 27005). Each risk links an asset, a threat and a vulnerability, is scored, treated, mapped to Annex A controls, and re-scored as residual risk. The same scales are used throughout the project.

## 2. Likelihood
| Score | Description |
|---|---|
| 1 | Rare |
| 2 | Unlikely |
| 3 | Possible |
| 4 | Likely |
| 5 | Almost Certain |

## 3. Impact
| Score | Description |
|---|---|
| 1 | Insignificant |
| 2 | Minor |
| 3 | Moderate |
| 4 | Major |
| 5 | Severe |

## 4. Calculation
`Risk Score = Likelihood x Impact`

| Score | Rating |
|---|---|
| 1-4 | Low |
| 5-9 | Medium |
| 10-16 | High |
| 17-25 | Critical |

## 5. Risk appetite and acceptance (portfolio assumption)
- Critical and High risks must be treated; they cannot be accepted.
- Residual Medium risks may be accepted by the Risk Owner with Security Lead approval.
- Residual Medium risks with Impact 5 are escalated to management.
- Low risks are accepted and monitored.

## 6. Process
1. Identify assets and their C/I/A values (`Asset-Inventory.xlsx`).
2. Identify threats and vulnerabilities per asset.
3. Score inherent risk.
4. Select treatment: mitigate, transfer, avoid or accept.
5. Map to Annex A controls (`Control-Mapping.xlsx`) and record in the SoA.
6. Score residual risk after the planned treatment.
7. Review risks at least annually and after significant change or incident.

## 7. Roles
| Role | Responsibility |
|---|---|
| Risk Owner | Accepts or treats the risk, delivers actions |
| Security Lead | Maintains methodology and register |
| Management | Approves risk acceptance above appetite and treatment resources |

## 8. Review history
| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | Oct 2026 | Initial release | Security Lead |
