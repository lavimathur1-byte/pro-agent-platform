Version 0.1 \| Status: requirements baseline, not approval to deploy \| Owner: Founder \| Geography: Dubai-first

# 01 \| Product brief

A Dubai-first PRO and company-administration services business supported by an internal operating system. It sells scoped, transparently quoted service work and recurring SME retainers. The platform maintains a single customer/case record, logs approvals and evidence, coordinates authorised human processing, and uses narrowly permissioned AI assistants for repetitive low-risk activities. The system is not a government portal, legal adviser or autonomous compliance officer.

# 02 \| Founder-friendly operating contract

- Founder Lavi has zero programming experience. Explain every decision in plain English: objective, customer impact, one recommended default, alternatives, estimated cost, risk and approval needed. Define technical terms on first use.

- A coding agent must never infer approval from silence, spend money, open production access, handle real identity documents, change permissions or deploy to production without explicit founder approval.

- At the end of each small task provide: what changed, demonstration/screenshots, tests run with results, security impact, exact costs, open decisions and next task.

- When blocked, make a safe mock or stub and record blocker; do not invent legal answers, API access, government fees, external credentials or successful tests.

- Automated coding agents can write and run code but cannot substitute for an independent qualified reviewer for security, compliance or legal sign-off.

# 03 \| Shared scope and release principle

Initial assumption for planning: existing Dubai mainland SMEs of 5–25 staff. Candidate initial services: licence renewal; employment entry permit; residence permit issuance and renewal; visa cancellation; Emirates ID issuance and renewal; work-permit issuance; establishment-card handling; document attestation. Exact list, categorization and permission are unapproved until P00. The reports differ on priority; founder must choose explicitly. Formation and free-zone coverage remain a validated backlog, not silently included in launch.

Delivery strategy: core security/data/audit foundations from the first increment; manual government processing and compliance decisions; use bought CRM/accounting/payment/identity where appropriate. Defer full customer portal, mobile app, bespoke CRM/ERP, 18+ agents and government-portal automation.

# 04 \| Reconciling source studies: gap register

| ID / issue                                            | Observed gap                                                                                                                                          | Required resolution                                                                                                      |
|-------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| G01 Conflicting forecast and bootstrap envelope       | Two reports contain different five-year revenue, EBITDA and funding outputs. Neither is an approved product budget.                                   | Founder/finance selects baseline model, reconciles definitions and approves a spending cap before P01.                   |
| G02 Market differentiation overstated in first report | First report calls published pricing/portal gaps validated; second documents transparent-pricing and AI competitors.                                  | Treat differentiation as hypothesis; interviews and competitive checks, no first-mover claims.                           |
| G03 Conflicting MVP scope                             | First outlines web/portal stack; second advises no customer portal in year one and spreadsheet-first operations.                                      | Core structured record and audit history are non-negotiable; defer full portal until gate P07.                           |
| G04 Unverified legal permission                       | Specific licence activity, AML duties, authorised government channels, government portal automation and privacy obligations remain partly unresolved. | Legal counsel + compliance sign written gate; no live submissions or production personal data beforehand.                |
| G05 Founder as compliance officer not established     | One study places founder as MLRO without demonstrating eligibility, independence or capacity.                                                         | Qualified specialist confirms eligibility and appointment; no automatic assumption that founder can fill role.           |
| G06 AI proposal broader than operating readiness      | 18–19 agent concepts but second study recommends only three initially.                                                                                | Build bounded A3 customer service, A4 onboarding and A9 renewals; remaining agent registry future only.                  |
| G07 GitHub verification contradiction                 | One report says GitHub REST API verified 18 repos; other says API returned 403 and HTML was reviewed for 28.                                          | Treat research as provisional; lock versions, license/SBOM/security review and test real packages in CI.                 |
| G08 Conflicting fee classifications                   | Medical, renewal and visa fee sources disagree and some numbers may mix components.                                                                   | Fee line items need official source URL, verified date, approver, effective period; unknown prices require manual quote. |
| G09 Insufficient operational control specification    | No complete case schema, invariant definitions, approval ownership or recovery procedures.                                                            | Introduce explicit data model, state transitions, maker-checker, event logging and recovery.                             |
| G10 Missing delivery governance                       | No complete definition of done, test pyramid, branch rules, vulnerability SLA or incident playbook.                                                   | Engineering policy applies to every phase and feature, not merely at launch.                                             |

# 05 \| Mandatory common guardrails

- Compliance gate: qualified local counsel and appropriately appointed compliance professional verify exact activity scope, AML/TCSP obligations, sanctioned activity, approved processing channels, notices, retention and data handling. Government automation disabled absent written authority.

- Human-only: final CDD/AML outcomes, beneficial-owner determinations, suspicious-activity reporting decisions, government submissions, legal/contractual commitments, money movement, bank details changes, refunds, employee decisions and final appeal decisions; confirm detailed legal allocation with counsel.

- Commercial controls: official fees and company service fees are separately labelled; sourced government fee version and receipt required; VAT/tax treatment and principal-versus-agent revenue recognition need accountant approval.

- Privacy: collect minimum necessary data, maintain processing inventory, perform vendor/data-transfer assessment, encrypt, restrict access, redact logs and set approved retention/deletion holds. UAE-region hosting is a preference pending legal review, not a claim of universal legal requirement.

- No production customer data in development, test, monitoring prompts, public repositories or third-party AI tools unless separately evaluated and approved. Default to synthetic fixtures.

- Research evidence labels: verified by source as of date; report claim; assumption; legally unconfirmed. Review owner, expiry and link must be recorded for each legal/fee/technology assertion.

# 06 \| Cross-document phase map

| Phase | Shared title                                     | Why this exists                                                                                                |
|-------|--------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| P00   | Decision gates and scope                         | Prevent software spending and live-data use before the permitted business model is known.                      |
| P01   | Project and engineering foundation               | Make every future change traceable, reviewable, reproducible and reversible.                                   |
| P02   | Identity, organizations and security             | Prevent one customer, agent or employee from viewing or changing another customer’s information.               |
| P03   | Service catalogue and transparent pricing        | Ensure customers can see the deliverable and distinguish service charges from third-party fees.                |
| P04   | Lead, onboarding and case record                 | Create one authoritative history from enquiry to delivery rather than disconnected chats and spreadsheets.     |
| P05   | Human-led service delivery and finance           | Prove accurate case completion, transparent billing and separation of duties before automation scales.         |
| P06   | Three bounded AI agents                          | Reduce repetitive work while keeping judgment, sensitive actions and external commitments under human control. |
| P07   | Customer communication and controlled visibility | Give customers reliable progress information without claiming government work is complete prematurely.         |
| P08   | Management metrics and audit                     | Measure actual service quality, customer outcomes, agent errors and unit economics from recorded events.       |
| P09   | Enterprise assurance and release                 | Demonstrate the system is secure, reliable and recoverable before real customers depend on it.                 |
| P10   | Pilot, learn and expand                          | Validate workflow and economics on actual cases before increasing automation or service coverage.              |

# 07 \| Implementation phases: common sequence

# P00 Decision gates and scope

WHY WE BUILD THIS PHASE: Prevent software spending and live-data use before the permitted business model is known.

## P00.00.1 Approve launch scope

Business requirement: Decide Dubai mainland first, existing SMEs 5–25 employees and initial eight services; record any changes in decision log.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 00.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P00.00.2 Legal and channel verification

Business requirement: Obtain written legal/activity, AML classification, government channel, privacy and third-party terms review; identify accountable approvers.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 00.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P00.00.3 Economics and pilot

Business requirement: Approve one forecast version, spending ceiling, pricing assumptions and a manual pilot to measure actual case work.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 00.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: Written licensing/channel/privacy/AML scope and budget approvals are attached; otherwise no production work.

# P01 Project and engineering foundation

WHY WE BUILD THIS PHASE: Make every future change traceable, reviewable, reproducible and reversible.

## P01.01.1 Repository and access

Business requirement: Create private GitHub repository, owner MFA, separate developer accounts, CODEOWNERS, protected main and PR template.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 01.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P01.01.2 Project skeleton

Business requirement: Create TypeScript monorepo, Next.js web, API application, shared validation schemas, PostgreSQL migrations, local development setup.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 01.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P01.01.3 CI and documentation

Business requirement: Set up lint/typecheck/unit tests/build/security scanners, dependency lockfiles, environment template and decision register.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 01.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P02 Identity, organizations and security

WHY WE BUILD THIS PHASE: Prevent one customer, agent or employee from viewing or changing another customer’s information.

## P02.02.1 Authentication

Business requirement: Use managed identity with MFA for staff, secure sessions and customer login; no custom password system.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 02.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P02.02.2 Authorization

Business requirement: Enforce tenant isolation and role permissions on server and database; define founder, compliance, PRO, coordinator, finance, customer and agent roles.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 02.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P02.02.3 Privacy baseline

Business requirement: Classify data, establish consent/notices, region and vendor review, retention schedule, encrypted storage, access logging and deletion workflows.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 02.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P03 Service catalogue and transparent pricing

WHY WE BUILD THIS PHASE: Ensure customers can see the deliverable and distinguish service charges from third-party fees.

## P03.03.1 Catalogue

Business requirement: Create versioned services by emirate, jurisdiction, eligibility, checklist, exclusions, SLA and approved source.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 03.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P03.03.2 Pricing

Business requirement: Model service fee, official fees, other pass-through charges and applicable tax as separate versioned lines; manual verified official-fee updates.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 03.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P03.03.3 Quote approvals

Business requirement: Produce dated quote with expiry and assumptions; discounts, exceptions and commitments require designated human approval.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 03.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P04 Lead, onboarding and case record

WHY WE BUILD THIS PHASE: Create one authoritative history from enquiry to delivery rather than disconnected chats and spreadsheets.

## P04.04.1 Lead capture

Business requirement: Website forms and CRM integration with deduplication, communication preferences and assigned owner.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 04.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P04.04.2 Onboarding

Business requirement: Secure document request/upload, checklist and human verification; prevent moving forward until compliance approval.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 04.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P04.04.3 Case workflow

Business requirement: Build explicit state machine, task ownership, deadlines, event log, external submission reference and controlled exception paths.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 04.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P05 Human-led service delivery and finance

WHY WE BUILD THIS PHASE: Prove accurate case completion, transparent billing and separation of duties before automation scales.

## P05.05.1 Operations

Business requirement: Prepare submission pack; authorised human submits via permitted channel, records receipt and government decision.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 05.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P05.05.2 Quality and exceptions

Business requirement: Four-eyes review for sensitive changes; rejection, resubmission, complaint and refund paths with named human owners.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 05.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P05.05.3 Finance integration

Business requirement: Buy accounting and gateway; link invoices, receipts, customer payments, pass-through fee reconciliations and approval-controlled refunds.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 05.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P06 Three bounded AI agents

WHY WE BUILD THIS PHASE: Reduce repetitive work while keeping judgment, sensitive actions and external commitments under human control.

## P06.06.1 Customer status agent

Business requirement: Answer only using authorised case data and reviewed knowledge; show source/version, escalate uncertainty or complaint.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 06.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P06.06.2 Onboarding agent

Business requirement: Explain checklist, classify uploads, extract fields into draft records; human verifies identity and compliance outcomes.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 06.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P06.06.3 Renewal agent

Business requirement: Create reminders and draft outreach from verified expiry dates; respect preferences, template approvals and human escalation.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 06.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P07 Customer communication and controlled visibility

WHY WE BUILD THIS PHASE: Give customers reliable progress information without claiming government work is complete prematurely.

## P07.07.1 Messaging

Business requirement: Integrate official WhatsApp provider or email behind adapter, consent/template control and message logs.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 07.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P07.07.2 Status view

Business requirement: Provide secure minimal case-status page only when tested demand and budget gate approve; otherwise verified email/WhatsApp updates.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 07.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P07.07.3 Notifications

Business requirement: Send threshold-based SLA alerts, missing-document requests and verified completion notices with deduplication.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 07.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P08 Management metrics and audit

WHY WE BUILD THIS PHASE: Measure actual service quality, customer outcomes, agent errors and unit economics from recorded events.

## P08.08.1 Event-derived KPIs

Business requirement: Define formulas, numerator/denominator, exclusions, owner, cadence and data lineage for key metrics.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 08.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P08.08.2 Dashboards

Business requirement: Ship role-scoped operational dashboard then founder view; do not expose individual personal documents in analytics.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 08.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P08.08.3 Audit and reconciliation

Business requirement: Produce tamper-evident event chain/export, approval register, reconciliation exception queue and evidence archive.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 08.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P09 Enterprise assurance and release

WHY WE BUILD THIS PHASE: Demonstrate the system is secure, reliable and recoverable before real customers depend on it.

## P09.09.1 Security verification

Business requirement: Threat model and map OWASP ASVS 5.0.0 Level 2 target controls, access and agent abuse tests; independent review.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 09.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P09.09.2 Reliability

Business requirement: Verify backup restore, incident response, monitoring, rate limiting, migration rollback and disaster-recovery drill.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 09.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P09.09.3 Release sign-off

Business requirement: Run full E2E and regression with synthetic data, production checklist, manual UAT and documented approvals.

Accountable decision: Founder + independent compliance/legal adviser

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 09.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P10 Pilot, learn and expand

WHY WE BUILD THIS PHASE: Validate workflow and economics on actual cases before increasing automation or service coverage.

## P10.10.1 Controlled pilot

Business requirement: Onboard limited approved customers, time every handoff, record issue and interruption and reconcile every case.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 10.1, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P10.10.2 Evidence-based improvements

Business requirement: Prioritize backlog using missed SLAs, rework, documented customer requests and privacy/security risks.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 10.2, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

## P10.10.3 Expansion gate

Business requirement: Consider portal, more agents, services and jurisdictions only on founder/compliance sign-off and proven unit economics.

Accountable decision: Founder + named department owner; compliance co-signs where customer data, regulated operations or fees change.

Business acceptance: named process owner confirms workflow in a plain-language demonstration, evidence is linked to requirement 10.3, unresolved legal or cost questions stay blocked, and a human can recover from a failure.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# 08 \| Stakeholders and decision rights

| Role                               | Accountability                                                              | Cannot delegate to agent                     |
|------------------------------------|-----------------------------------------------------------------------------|----------------------------------------------|
| Founder / sponsor                  | Budget, pricing, scope, go/no-go, customer experience                       | Contracts, production and spending approvals |
| Operations lead / authorised PRO   | Case ownership, government-channel SOP, service delivery                    | Official submissions and exceptions          |
| Compliance officer / legal counsel | AML applicability and decisions, regulatory interpretation, incident advice | Statutory judgment and filings               |
| Finance / qualified accountant     | Fee treatment, invoicing, reconciliation, taxes                             | Payments, refunds and accounting sign-off    |
| Security/engineering reviewer      | Independent code/security review and deployment checklist                   | Independent approval of own code             |
| Customer                           | Consent, upload, acknowledge quotation, query status                        | Cannot approve internal regulatory decisions |

# 09 \| Business data and KPIs

| Entity                | Minimum fields / rule                                                                                |
|-----------------------|------------------------------------------------------------------------------------------------------|
| Organization/customer | Tenant, contact, authority and consent basis, owner, status                                          |
| Person/document       | Sensitive identifiers restricted; file metadata and encrypted object references; access/review log   |
| Case/task             | Service/version, customer, assigned owner, status, clocks, dependencies, third-party reference       |
| Quote/invoice/receipt | Separate fee classes, approved source/effective date, tax configuration and reconciliation reference |
| Evidence / event      | Actor human or agent, action, timestamp, source version, approval, before/after safe metadata        |
| Agent execution       | Prompt/version, approved tools, inputs classified, output, tokens/cost, escalation, human verdict    |

KPI definitions require baseline and denominator, not merely target: quote turnaround (business hours), first-pass completeness (audited sample), SLA achievement (completed cases with pauses/exclusions logged), official rejection reasons, rework rate, gross margin per service after directly attributable cost, reconciliation exceptions, renewal reminder delivery, customer satisfaction, agent factual-error rate, human override rate and cost per case. Targets in source studies are hypotheses until piloted.

# 10 \| Business risks and controls

| Risk                                    | Preventive control                                                     | Detection / owner                                 |
|-----------------------------------------|------------------------------------------------------------------------|---------------------------------------------------|
| Wrong license / wrong government access | Written licence and channel gate; never scrape government portals      | Compliance review before each service enablement  |
| AML/KYC failure                         | Qualified compliance owner; manual decision; risk-based documented SOP | Compliance exception queue and independent audit  |
| Data breach / cross-tenant leak         | Default-deny access, encryption, vendor controls, least privilege      | Security alerts and incident owner                |
| Incorrect quote / fee                   | Approved versioned rates, expiry and human exceptions                  | Finance reconciliation and fee discrepancy report |
| Missed renewal                          | Verified expiry, owner, reminder ladder and escalation                 | Overdue dashboard and daily reconciliation        |
| AI invented advice or status            | Record-grounded responses, confidence failure =\> handoff              | Sample audit, complaint review, kill switch       |
| Excess spending / scope creep           | Budget limits and change register                                      | Founder monthly spend reconciliation              |

# 11 \| Assumptions, out-of-scope and stage funding

Not approved facts: customer demand, conversion, churn, throughput, quoted development cost, specific external service prices and local legal applicability. Financial report A and B are alternative assumptions and must not be averaged or substituted for a detailed line-item procurement budget. Set cap, owner, contingency and vendor quotes for each phase before spending. No calendar completion date is promised until team, licenses and integrations are confirmed.

Exclude from launch unless founder records change approval: proprietary government integrations, automated government filing, customer fund transfers by AI, tax or legal advice by unlicensed persons, mobile app, broad jurisdictions, bespoke accounting/CRM, client-facing autonomous AI decisions, unsupported language/OCR claims and ISO/SOC certification claims.

# 12 \| Founder approval questions: answer by selecting one option

- Confirm first launch offer: existing-SME recurring services, formation-led, or parallel pilot? Default planning assumption = existing SMEs.

- Who is the qualified compliance lead, and what written advice confirms activity/AML/channel/data obligations? Until named = BLOCKED.

- What is the maximum software budget and monthly running-cost ceiling, separately from company startup capital? Default = no paid provisioning.

- Does the founder approve a portal for pilot? Default = no, use verified messaging and internal case record.

- Which CRM, accounting, identity, storage, hosting and AI vendors have passed legal/security/cost review? Default = vendor-neutral adapters.

- Who will independently review PRs and security? A second human reviewer is required; if none, do not deploy live.

# 13 \| Business completion definition

The BRD is considered approved only after its scope, legal gates, financial baseline, RACI, pilot target and evidence owners are signed. The software is business-ready only when an authorised human can demonstrate an end-to-end case, all money and records reconcile, all customer commitments are supported by records, and the independent security/recovery gates pass.

# References and provenance

\[S1\] Consolidated report A: Pasted markdown.md, 16 Sep 2026; internal study, assumptions not independently re-verified for this document.

\[S2\] Consolidated report B: Pasted markdown(1).md, 16 Sep 2026; internal study and documented limitations, not legal sign-off.

\[S3\] OWASP ASVS 5.0.0: https://owasp.org/www-project-application-security-verification-standard/ ; stable baseline, accessed 16 Sep 2026.

\[S4\] GitHub rulesets: https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/available-rules-for-rulesets ; actual functionality varies by plan.

\[S5\] GitHub PR governance: https://docs.github.com/en/pull-requests/reference/managing-and-standardizing-pull-requests ; templates, CODEOWNERS, protected branches.

\[S6\] UAE authority sources: Obtain dated official DET, MOHRE, GDRFA, ICP, FTA, Ministry and data-protection guidance and written professional advice before enabling regulated flows; exact rules not certified here.

This document distinguishes research claims from confirmed production requirements. It is not a legal opinion, independent penetration-test report or confirmed vendor procurement estimate.
