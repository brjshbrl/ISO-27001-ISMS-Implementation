# ISO/IEC 27001:2022 ISMS Implementation – HawkPay Technologies (Simulated)

> **Simulated portfolio project.** HawkPay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

A GRC portfolio project that builds an ISO/IEC 27001:2022-aligned ISMS for a fictional 50-person FinTech/SaaS company (AWS, Microsoft 365, GitHub, PostgreSQL, CRM, HR/payroll SaaS).

**At a glance:** 20 assets · 18 risks (1 🔴 Critical, 17 🟠 High → all Medium or below after treatment) · 93 Annex A controls · 7 policies · 4 audit findings · management review with KPIs

> 📊 **GitHub can't preview `.xlsx` files**, so every workbook is also shown below and exported as CSV in [`csv-views/`](csv-views/) (click any CSV to view it as a table). Download the `.xlsx` files for formulas and filters.

## Lifecycle
Context → Scope → Assets → Risk Assessment → Risk Treatment → Control Mapping → SoA → Policies → Gap Assessment → Internal Audit → Corrective Actions → Management Review → Continual Improvement

**Traceability:** `Asset (02) → Risk (03) → Treatment (03) → ISO control (04) → Evidence (07) → Audit result (07) → Corrective action (08) → Management review (09)`

## Repository contents
| Folder | Contents |
|---|---|
| [01-ISMS-Scope](01-ISMS-Scope/) | Scope statement, issues, interested parties, legal and regulatory obligations |
| [02-Asset-Management](02-Asset-Management/) | 20 assets with owner, classification, C/I/A (criticality = MAX by formula) |
| [03-Risk-Management](03-Risk-Management/) | 5×5 methodology, 18-risk register with residual scoring, treatment plan |
| [04-ISO-Controls](04-ISO-Controls/) | Risk-to-Annex A mapping; Statement of Applicability (all 93 controls) |
| [05-Policies](05-Policies/) | 7 policies with document control |
| [06-Gap-Assessment](06-Gap-Assessment/) | Current vs target state and severity |
| [07-Internal-Audit](07-Internal-Audit/) | Checklist, findings, evidence register |
| [08-Corrective-Actions](08-Corrective-Actions/) | Root cause, action, owner, deadline |
| [09-Management-Review](09-Management-Review/) | KPIs and management decisions |

## Risk register (preview)
Method: Risk = Likelihood × Impact (5×5). 1–4 Low · 5–9 Medium · 10–16 High · 17–25 Critical. Full register: [`Risk-Register.xlsx`](03-Risk-Management/Risk-Register.xlsx) / [CSV](csv-views/Risk-Register.csv)

| ID | Asset | Threat | Vulnerability | L×I | Score | Rating | Residual | Owner | Status |
|---|---|---|---|---|---|---|---|---|---|
| R-001 | Customer DB | Data breach | Excessive privileges | 4×5 | 20 | 🔴 Critical | 8 (Medium) | CTO | Open |
| R-002 | AWS | Cloud compromise | Misconfigured IAM | 3×5 | 15 | 🟠 High | 8 (Medium) | DevOps Lead | Open |
| R-003 | GitHub | Account takeover | MFA not enforced | 3×5 | 15 | 🟠 High | 5 (Medium) | Engineering Lead | In Progress |
| R-004 | Laptops | Malware | Weak endpoint controls | 4×4 | 16 | 🟠 High | 6 (Medium) | IT Manager | In Progress |
| R-005 | M365 | Phishing | Limited awareness | 4×4 | 16 | 🟠 High | 9 (Medium) | HR / Security Lead | Open |
| R-006 | VPN | Unauthorized access | Weak authentication | 3×5 | 15 | 🟠 High | 8 (Medium) | IT Manager | Open |
| R-007 | Backup | Data loss | Inadequate backup testing | 3×5 | 15 | 🟠 High | 8 (Medium) | DevOps Lead | Open |
| R-008 | API Keys | Credential exposure | Poor secret management | 3×5 | 15 | 🟠 High | 8 (Medium) | DevOps Lead | Open |
| R-009 | HR System | Data disclosure | Excessive access | 3×4 | 12 | 🟠 High | 6 (Medium) | HR Manager | Open |
| R-010 | Customer Support | Data leakage | Improper data handling | 3×4 | 12 | 🟠 High | 6 (Medium) | Support Lead | Open |
| R-011 | Source Code | Intellectual property theft | Excessive repository access | 3×4 | 12 | 🟠 High | 6 (Medium) | Engineering Lead | Open |
| R-012 | AWS | Service outage | Single-region dependency | 3×5 | 15 | 🟠 High | 8 (Medium) | DevOps Lead | Open |
| R-013 | Security Logs | Evidence loss | Insufficient retention | 3×4 | 12 | 🟠 High | 6 (Medium) | Security Lead | Open |
| R-014 | Employee Laptop | Data theft | Disk encryption gap | 3×4 | 12 | 🟠 High | 4 (Low) | IT Manager | Open |
| R-015 | Vendor | Supply-chain compromise | Weak vendor assessment | 3×5 | 15 | 🟠 High | 8 (Medium) | Procurement | Open |
| R-016 | Website | Exploitation | Unpatched components | 3×4 | 12 | 🟠 High | 6 (Medium) | IT Manager | Open |
| R-017 | Payroll Data | Unauthorized disclosure | Weak access segregation | 2×5 | 10 | 🟠 High | 5 (Medium) | Finance Manager | Open |
| R-018 | Network | Lateral movement | Poor segmentation | 3×4 | 12 | 🟠 High | 6 (Medium) | DevOps Lead | Open |

## Risk treatment (highest-priority actions)
Full plan: [`Risk-Treatment-Plan.xlsx`](03-Risk-Management/Risk-Treatment-Plan.xlsx)

| Risk | Treatment action | Owner | Due | Annex A |
|---|---|---|---|---|
| R-001 | Conduct quarterly database access reviews; remove standing admin access | CTO | 30 days | A.5.15, A.5.18, A.8.2 |
| R-002 | Review AWS IAM permissions; enable IAM Access Analyzer | DevOps Lead | 30 days | A.5.23, A.8.2 |
| R-003 | Enforce MFA on GitHub org | Engineering Lead | 15 days | A.5.17, A.8.5 |
| R-004 | Deploy endpoint protection (EDR) on all laptops | IT Manager | 45 days | A.8.7, A.8.1 |
| R-005 | Conduct phishing simulation and security awareness training | HR / Security Lead | 30 days | A.6.3, A.8.23 |
| R-006 | Enforce MFA on VPN | IT Manager | 30 days | A.5.15, A.8.5 |
| R-007 | Perform quarterly backup restoration test | DevOps Lead | 30 days | A.8.13 |
| R-008 | Move secrets to AWS Secrets Manager; enable GitHub secret scanning | DevOps Lead | 45 days | A.5.17, A.8.24 |

## Asset inventory (preview)
Full inventory: [`Asset-Inventory.xlsx`](02-Asset-Management/Asset-Inventory.xlsx) / [CSV](csv-views/Asset-Inventory.csv)

| ID | Asset | Owner | Class. | C | I | A | Criticality |
|---|---|---|---|---|---|---|---|
| AST-001 | Customer Database | CTO | Restricted | 5 | 5 | 5 | 5 |
| AST-002 | Payment Application | CTO | Confidential | 4 | 5 | 5 | 5 |
| AST-003 | AWS Production Environment | DevOps Lead | Restricted | 5 | 5 | 5 | 5 |
| AST-004 | GitHub Repository | Engineering Lead | Confidential | 4 | 5 | 4 | 5 |
| AST-005 | Microsoft 365 | IT Manager | Confidential | 4 | 4 | 4 | 4 |
| AST-006 | Employee Laptops | IT Manager | Internal | 3 | 3 | 3 | 3 |
| AST-007 | VPN | IT Manager | Confidential | 4 | 4 | 4 | 4 |
| AST-008 | Firewall | IT Manager | Confidential | 3 | 5 | 5 | 5 |
| AST-009 | Company Website | Marketing | Public | 2 | 4 | 4 | 4 |
| AST-010 | CRM System | Sales Manager | Confidential | 4 | 3 | 3 | 4 |
| AST-011 | HR Management System | HR Manager | Confidential | 4 | 4 | 3 | 4 |
| AST-012 | Payroll Data | Finance Manager | Restricted | 5 | 5 | 3 | 5 |
| AST-013 | Backup Repository | DevOps Lead | Restricted | 5 | 5 | 4 | 5 |
| AST-014 | Source Code Repository (data view) | Engineering Lead | Confidential | 4 | 5 | 3 | 5 |
| AST-015 | Employee Directory | HR Manager | Internal | 2 | 3 | 2 | 3 |
| AST-016 | Security Logs | Security Lead | Restricted | 4 | 5 | 3 | 5 |
| AST-017 | API Keys / Secrets | DevOps Lead | Restricted | 5 | 5 | 4 | 5 |
| AST-018 | Customer Support Platform | Support Lead | Confidential | 4 | 3 | 4 | 4 |
| AST-019 | Security Documentation | Security Lead | Internal | 2 | 3 | 2 | 3 |
| AST-020 | Vendor Contracts | Legal/Finance | Confidential | 4 | 4 | 2 | 4 |

## Mock internal audit results
| Control | Question | Result |
|---|---|---|
| A.5.9 | Are assets inventoried? | ✅ Pass |
| A.5.15 | Are access rights reviewed? | 🟡 Partial |
| A.5.17 | Is MFA enforced? | 🟡 Partial |
| A.8.13 | Are backups tested? | ❌ Fail |
| A.5.1 | Are security policies approved? | ✅ Pass |
| A.5.24 | Are incidents documented? | ✅ Pass |
| A.5.19 | Are vendors assessed? | 🟡 Partial |

| Finding | Control | Severity | Corrective action | Owner | Due |
|---|---|---|---|---|---|
| AF-001 | A.8.13 | Major | Quarterly backup restoration testing with evidence | DevOps Lead | 30 days |
| AF-002 | A.5.17 | Major | Enforce MFA for all users (82% today) | IT Manager | 15 days |
| AF-003 | A.5.19 | Minor | Vendor security assessment questionnaire | Procurement | 60 days |
| AF-004 | A.5.15 | Minor | Quarterly privileged-access reviews | CTO | 30 days |

## Management review KPIs (fictional)
| KPI | Value | Target |
|---|---|---|
| MFA coverage | 82% | 100% |
| Security training completion | 94% | 95% |
| Open Critical / High risks | 1 / 17 | 0 / ≤5 |
| Critical vulnerabilities >30 days | 2 | 0 |
| Access reviews completed | 75% | 100% |
| Incident response SLA | 91% | 95% |
| Backup restore tests completed | 0 | 4 per year |

## Skills demonstrated
Governance, risk management, ISO 27001 clause and Annex A knowledge, audit evidence, corrective action, management reporting.

## Limitations
Fictional company, simulated evidence and KPIs. Legal obligations are identified, not assessed. Not a certification claim.
