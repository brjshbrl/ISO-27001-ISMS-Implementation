# Access Control Policy

> **Simulated portfolio project.** SecurePay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

| Document control | |
|---|---|
| **Document ID** | SP-ISMS-POL-002 |
| **Version** | 1.0 |
| **Owner** | IT Manager |
| **Approved By** | CEO (simulated) |
| **Effective Date** | 08 October 2026 |
| **Review Date** | 08 October 2027 (annual) |
| **Classification** | Internal |
| **Related controls** | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.4, A.8.5 |

## 1. Purpose
To ensure access to information and systems is authorised, least-privilege and traceable.

## 2. Scope
All employees, contractors and third parties accessing SecurePay information or systems within the ISMS scope (see `01-ISMS-Scope/ISMS-Scope.md`).

## 3. Responsibilities
| Role | Responsibility |
|---|---|
| IT Manager | Operate identity lifecycle and MFA |
| System / Asset Owners | Approve access and perform periodic reviews |
| HR | Trigger joiner, mover and leaver processes |
| Users | Protect credentials and use access only for business purposes |

## 4. Requirements
1. Access is granted on a need-to-know, least-privilege basis and approved by the asset owner.
2. Every user has a unique identity; shared accounts are prohibited.
3. MFA is mandatory for M365, GitHub, VPN, AWS and all administrative access.
4. Privileged access is separate from standard accounts, time-bound where possible, and logged.
5. Joiners receive role-based access; movers have access re-evaluated; leavers are disabled on the last working day.
6. User access and privileged access are reviewed quarterly; reviews are evidenced and exceptions removed within 5 working days.
7. Passwords/passphrases follow minimum length and are never reused; secrets are stored only in the approved vault.
8. Access to source code and production data is restricted to named roles.

## 5. Exceptions
Exceptions must be requested in writing, risk-assessed, approved by the Security Lead (and the CEO for High risks), time-limited (maximum 6 months) and recorded in the exceptions log. Non-compliance may lead to disciplinary action under HR policy.

## 6. Review History
| Version | Date | Change | Author | Approver |
|---|---|---|---|---|
| 1.0 | 08 Oct 2026 | Initial release | IT Manager | CEO (simulated) |
