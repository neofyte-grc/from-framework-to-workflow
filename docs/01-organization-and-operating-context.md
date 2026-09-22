# Organization and Operating Context

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Document owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Organization Profile

Peachtree Logistics Group is a fictional regional logistics company headquartered in Atlanta, Georgia.

PLG employs approximately 225 personnel and provides:

- Warehousing
- Last-mile delivery
- Medical courier services
- Freight brokerage
- Regional transportation coordination

PLG serves customers throughout the southeastern United States. Its operations depend on rapid communication, accurate scheduling, mobile technology, third-party coordination, and continuous access to business systems.

---

## 2. Business Model

PLG coordinates the movement of goods and information between:

- Commercial customers
- Healthcare clients
- Warehouses
- Dispatch personnel
- Employed drivers
- Independent couriers
- Shipment recipients
- Technology vendors
- Payment processors
- Financial institutions

Access to systems and information must support time-sensitive work without granting unnecessary permissions.

---

## 3. Workforce Groups

| Workforce group | Primary responsibilities | Typical access needs | IAM considerations |
| --- | --- | --- | --- |
| Executive leadership | Strategy, finance, oversight, and risk decisions | Reports, financial information, governance records | High-value accounts and sensitive information |
| Office staff | Administration, customer support, HR, and records | Microsoft 365, shared files, business applications | Oversharing and accumulated access |
| Dispatch staff | Scheduling, assignment, and delivery coordination | Dispatch platform, customer data, driver information | Time-sensitive access and shift coverage |
| Warehouse staff | Inventory, storage, scanning, and release | WMS, scanners, facility access | Shared work areas and shift changes |
| Employed drivers | Pickup, delivery, and status reporting | Delivery application and assigned records | Mobile access outside PLG facilities |
| Independent couriers | Assigned delivery services | Limited delivery assignments | Identity separation, expiration, and vendor-style access |
| Finance staff | Billing, reconciliation, and payment processing | Billing system and financial records | Segregation-of-duties concerns |
| IT personnel | Support, administration, and configuration | Administrative access across systems | Privileged-access governance |
| Contractors and vendors | Specialized or temporary services | Limited system or facility access | Sponsorship, duration, and monitoring |

---

## 4. Technology Environment

PLG operates a mixed cloud and on-premises environment.

### 4.1 Microsoft 365

Microsoft 365 supports:

- Email
- Microsoft Teams
- SharePoint
- Document collaboration
- Calendar functions
- Administrative communications

### 4.2 Logistics and Freight Platform

The cloud logistics and freight brokerage platform supports:

- Order intake
- Shipment records
- Freight coordination
- Customer information
- Carrier information
- Delivery status
- Operational reporting

### 4.3 Warehouse Management System

The on-premises warehouse management system supports:

- Inventory tracking
- Receiving
- Storage location
- Picking
- Release
- Warehouse scanning
- Shipment preparation

### 4.4 Dispatch and Delivery Platform

The dispatch and delivery platform supports:

- Driver and courier assignment
- Route information
- Pickup instructions
- Delivery instructions
- Status updates
- Delivery confirmation
- Exception reporting

### 4.5 Billing and Accounting System

The billing and accounting system supports:

- Invoicing
- Customer accounts
- Payment records
- Reconciliation
- Financial reporting
- Vendor payments

### 4.6 Devices

PLG uses:

- Company-managed laptops
- Company-managed mobile devices
- Warehouse scanners
- Shared operational workstations
- Approved personal mobile devices
- Remote-access capabilities
- Physical-access badges and keys

---

## 5. Information Types

| Information category | Examples | Primary concern |
| --- | --- | --- |
| Workforce information | Employment status, contact information, role, schedule | Privacy and unauthorized access |
| Customer information | Names, contacts, contracts, service details | Confidentiality and contractual obligations |
| Delivery information | Addresses, routes, status, recipient details | Privacy, integrity, and operational reliability |
| Medical-delivery information | Healthcare client information and PHI/ePHI flags | Heightened privacy and handling requirements |
| Financial information | Invoices, payments, account records | Fraud and unauthorized disclosure |
| Vendor information | Contracts, contacts, services, access details | Third-party and supply-chain risk |
| Authentication information | Accounts, credentials, tokens, MFA records | Account compromise |
| Authorization information | Roles, groups, permissions, approvals | Excessive or unauthorized access |
| Audit information | Logs, tickets, reviews, and evidence | Accountability and assessment integrity |

---

## 6. Core Business Processes

| Process ID | Business process | Supporting systems |
| --- | --- | --- |
| `P1` | Order intake | Microsoft 365 and logistics platform |
| `P2` | Review and scheduling | Logistics platform |
| `P3` | Dispatch and driver assignment | Dispatch platform |
| `P4` | Pickup and delivery | Delivery mobile application |
| `P5` | Delivery confirmation | Dispatch and logistics platforms |
| `P6` | Billing and record retention | Billing system and Microsoft 365 |

These processes depend on timely and accurate access. Excessive restrictions could disrupt delivery operations, while excessive permissions could expose sensitive data or allow unauthorized changes.

---

## 7. Operational Characteristics

PLG’s access-control design must account for:

- Multiple work shifts
- Time-sensitive delivery schedules
- Weekend and after-hours operations
- Temporary shift coverage
- Employee transfers
- Seasonal staffing
- Independent couriers
- Remote work
- Mobile access
- Shared physical workspaces
- Vendor-managed applications
- Medical-delivery handling
- Emergency operational changes

---

## 8. Trust Boundaries

Important trust boundaries exist between:

1. PLG employees and independent couriers
2. PLG-managed and personally owned devices
3. Cloud platforms and on-premises systems
4. Standard users and privileged administrators
5. General delivery data and medical-delivery information
6. PLG and its technology vendors
7. Internal applications and external payment processors
8. Warehouse systems and mobile delivery applications
9. Business operations and security administration
10. Requesters, approvers, provisioners, and reviewers

---

## 9. IAM Operating Challenges

PLG’s operating model creates several IAM challenges:

- Personnel may require access before the beginning of a shift.
- Role changes may occur faster than access reviews.
- Dispatch personnel may require temporary coverage permissions.
- Independent couriers should not be treated as employees.
- Contractor access must have a sponsor and expiration date.
- Shared workstations may weaken individual accountability.
- Vendor applications may not support centralized provisioning.
- Emergency access may be necessary during disruptions.
- Medical-delivery information requires more restrictive access.
- Managers may not understand technical entitlement names.
- Manual processes may create delayed removal and incomplete evidence.

---

## 10. Security and Business Priorities

The IAM program must balance:

- Operational continuity
- Least privilege
- Timely access
- Timely revocation
- Individual accountability
- Privacy
- Data protection
- Segregation of duties
- Contractor restrictions
- Evidence quality
- Control sustainability

The target operating model should help PLG deliver services reliably while reducing unauthorized access and improving accountability.

---

## 11. Context Conclusion

PLG’s environment requires an IAM model that is structured but operationally practical.

The program must support rapid logistics operations while ensuring that:

- Access is based on verified identity and business need.
- Permissions reflect current responsibilities.
- High-risk access receives stronger review.
- Departed personnel lose access promptly.
- Independent couriers remain separated from employees.
- Sensitive data receives appropriate protection.
- Control activities produce reliable evidence.
- Failures are detected and escalated.
