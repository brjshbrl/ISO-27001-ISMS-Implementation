# Backup & Recovery Policy

> **Simulated portfolio project.** HawkPay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

| Document control | |
|---|---|
| **Document ID** | HP-ISMS-POL-006 |
| **Version** | 1.0 |
| **Owner** | DevOps Lead |
| **Approved By** | CEO (simulated) |
| **Effective Date** | 08 October 2026 |
| **Review Date** | 08 October 2027 (annual) |
| **Classification** | Internal |
| **Related controls** | A.8.13, A.8.14, A.5.29, A.5.30 |

## 1. Purpose
To ensure critical data and systems can be recovered within agreed objectives.

## 2. Scope
Production databases, application configuration, source code, M365 data and security logs within ISMS scope.

## 3. Responsibilities
| Role | Responsibility |
|---|---|
| DevOps Lead | Operate backups, run restoration tests, keep evidence |
| Asset Owners | Define RPO/RTO for their assets |
| Security Lead | Review test results and report to management |

## 4. Requirements
1. Backup frequency: customer database daily with point-in-time recovery; configuration and code continuously/versioned (targets to be confirmed per asset).
2. Backups are encrypted, stored separately from production (separate account/bucket) and access-restricted.
3. Retention follows the retention schedule defined per asset in the Asset Inventory.
4. Restoration tests are performed at least quarterly and results retained as evidence.
5. Failed backups or tests are logged as incidents and tracked to closure.
6. Recovery objectives (RPO/RTO) are defined and tested against the DR plan.

## 5. Exceptions
Exceptions must be requested in writing, risk-assessed, approved by the Security Lead (and the CEO for High risks), time-limited (maximum 6 months) and recorded in the exceptions log. Non-compliance may lead to disciplinary action under HR policy.

## 6. Review History
| Version | Date | Change | Author | Approver |
|---|---|---|---|---|
| 1.0 | 08 Oct 2026 | Initial release | DevOps Lead | CEO (simulated) |
