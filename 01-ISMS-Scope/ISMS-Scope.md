# ISMS Scope

> **Simulated portfolio project.** HawkPay Technologies Pvt. Ltd. is a fictional organisation. Nothing here claims real certification or legal compliance.

| | |
|---|---|
| **Organization** | HawkPay Technologies Pvt. Ltd. |
| **ISMS Version** | 1.0 |
| **Date** | October 2026 |
| **Standard** | ISO/IEC 27001:2022 (clause 4.3) |

## Scope Statement
The Information Security Management System of HawkPay Technologies Pvt. Ltd. covers the people, processes, information assets and technologies involved in the development, operation, maintenance and support of the company's cloud-based payment management platform.

The scope includes AWS production infrastructure, customer information, application source code, corporate endpoints, Microsoft 365, GitHub, business applications, IT support processes, information security processes and third-party services supporting the organization's operations.

## In Scope
| Area | Included |
|---|---|
| Cloud | AWS production environment |
| Applications | Payment management platform |
| Data | Customer and business information |
| Development | GitHub repositories / source code |
| Endpoints | Company laptops |
| Collaboration | Microsoft 365 |
| IT | Identity, access, network and support |
| Personnel | Employees and relevant contractors |
| Vendors | Critical technology suppliers |
| Security | Incident, vulnerability and access management |

## Out of Scope
| Area | Reason |
|---|---|
| AWS physical data centers | Managed by AWS; assurance obtained through supplier management (A.5.19-A.5.23) |
| Employee personal devices | Not used for production business processing |
| Personal email accounts | Outside corporate environment |
| Customer internal infrastructure | Outside HawkPay's control |

## Interfaces and dependencies
- AWS operates under the shared-responsibility model: HawkPay remains responsible for configuration, identity, data and applications.
- Exclusions are justified by control boundary, not convenience, and are reviewed annually.

## Related documents
`Interested-Parties.xlsx` (issues, interested parties, legal and regulatory requirements) | `../02-Asset-Management/Asset-Inventory.xlsx`
