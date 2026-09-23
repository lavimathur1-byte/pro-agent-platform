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

Coding-agent build instruction: Decide Dubai mainland first, existing SMEs 5–25 employees and initial eight services; record any changes in decision log.

Technical implementation: Deliver ADR (architecture decision record), scope checklist, evidence links, explicit gate state BLOCKED/APPROVED and approvals directory; prohibit production secrets until gate approved.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P00.00.2 Legal and channel verification

Coding-agent build instruction: Obtain written legal/activity, AML classification, government channel, privacy and third-party terms review; identify accountable approvers.

Technical implementation: Deliver ADR (architecture decision record), scope checklist, evidence links, explicit gate state BLOCKED/APPROVED and approvals directory; prohibit production secrets until gate approved.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P00.00.3 Economics and pilot

Coding-agent build instruction: Approve one forecast version, spending ceiling, pricing assumptions and a manual pilot to measure actual case work.

Technical implementation: Deliver ADR (architecture decision record), scope checklist, evidence links, explicit gate state BLOCKED/APPROVED and approvals directory; prohibit production secrets until gate approved.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: Written licensing/channel/privacy/AML scope and budget approvals are attached; otherwise no production work.

# P01 Project and engineering foundation

WHY WE BUILD THIS PHASE: Make every future change traceable, reviewable, reproducible and reversible.

## P01.01.1 Repository and access

Coding-agent build instruction: Create private GitHub repository, owner MFA, separate developer accounts, CODEOWNERS, protected main and PR template.

Technical implementation: Implement repository structure and CI as code; reproducible README setup, pinned dependencies and one-command local startup; required checks before PR merge.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P01.01.2 Project skeleton

Coding-agent build instruction: Create TypeScript monorepo, Next.js web, API application, shared validation schemas, PostgreSQL migrations, local development setup.

Technical implementation: Implement repository structure and CI as code; reproducible README setup, pinned dependencies and one-command local startup; required checks before PR merge.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P01.01.3 CI and documentation

Coding-agent build instruction: Set up lint/typecheck/unit tests/build/security scanners, dependency lockfiles, environment template and decision register.

Technical implementation: Implement repository structure and CI as code; reproducible README setup, pinned dependencies and one-command local startup; required checks before PR merge.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P02 Identity, organizations and security

WHY WE BUILD THIS PHASE: Prevent one customer, agent or employee from viewing or changing another customer’s information.

## P02.02.1 Authentication

Coding-agent build instruction: Use managed identity with MFA for staff, secure sessions and customer login; no custom password system.

Technical implementation: Enforce middleware plus database row-level/tenant filters, automated authorization tests and secure files with short-lived access URLs; deny by default.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P02.02.2 Authorization

Coding-agent build instruction: Enforce tenant isolation and role permissions on server and database; define founder, compliance, PRO, coordinator, finance, customer and agent roles.

Technical implementation: Enforce middleware plus database row-level/tenant filters, automated authorization tests and secure files with short-lived access URLs; deny by default.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P02.02.3 Privacy baseline

Coding-agent build instruction: Classify data, establish consent/notices, region and vendor review, retention schedule, encrypted storage, access logging and deletion workflows.

Technical implementation: Enforce middleware plus database row-level/tenant filters, automated authorization tests and secure files with short-lived access URLs; deny by default.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P03 Service catalogue and transparent pricing

WHY WE BUILD THIS PHASE: Ensure customers can see the deliverable and distinguish service charges from third-party fees.

## P03.03.1 Catalogue

Coding-agent build instruction: Create versioned services by emirate, jurisdiction, eligibility, checklist, exclusions, SLA and approved source.

Technical implementation: Use normalized, versioned catalogue and fee tables with effective_from/to and approver; monetary values in integer fils or fixed decimal, not floating point.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P03.03.2 Pricing

Coding-agent build instruction: Model service fee, official fees, other pass-through charges and applicable tax as separate versioned lines; manual verified official-fee updates.

Technical implementation: Use normalized, versioned catalogue and fee tables with effective_from/to and approver; monetary values in integer fils or fixed decimal, not floating point.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P03.03.3 Quote approvals

Coding-agent build instruction: Produce dated quote with expiry and assumptions; discounts, exceptions and commitments require designated human approval.

Technical implementation: Use normalized, versioned catalogue and fee tables with effective_from/to and approver; monetary values in integer fils or fixed decimal, not floating point.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P04 Lead, onboarding and case record

WHY WE BUILD THIS PHASE: Create one authoritative history from enquiry to delivery rather than disconnected chats and spreadsheets.

## P04.04.1 Lead capture

Coding-agent build instruction: Website forms and CRM integration with deduplication, communication preferences and assigned owner.

Technical implementation: Implement tenant-owned lead, organization, person, case, task, document metadata and immutable event records; explicit allowed transitions and idempotent writes.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P04.04.2 Onboarding

Coding-agent build instruction: Secure document request/upload, checklist and human verification; prevent moving forward until compliance approval.

Technical implementation: Implement tenant-owned lead, organization, person, case, task, document metadata and immutable event records; explicit allowed transitions and idempotent writes.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P04.04.3 Case workflow

Coding-agent build instruction: Build explicit state machine, task ownership, deadlines, event log, external submission reference and controlled exception paths.

Technical implementation: Implement tenant-owned lead, organization, person, case, task, document metadata and immutable event records; explicit allowed transitions and idempotent writes.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P05 Human-led service delivery and finance

WHY WE BUILD THIS PHASE: Prove accurate case completion, transparent billing and separation of duties before automation scales.

## P05.05.1 Operations

Coding-agent build instruction: Prepare submission pack; authorised human submits via permitted channel, records receipt and government decision.

Technical implementation: Persist receipt references, invoice reconciliation events and dual-approval flows; payment gateway handles card data, never our servers.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P05.05.2 Quality and exceptions

Coding-agent build instruction: Four-eyes review for sensitive changes; rejection, resubmission, complaint and refund paths with named human owners.

Technical implementation: Persist receipt references, invoice reconciliation events and dual-approval flows; payment gateway handles card data, never our servers.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P05.05.3 Finance integration

Coding-agent build instruction: Buy accounting and gateway; link invoices, receipts, customer payments, pass-through fee reconciliations and approval-controlled refunds.

Technical implementation: Persist receipt references, invoice reconciliation events and dual-approval flows; payment gateway handles card data, never our servers.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P06 Three bounded AI agents

WHY WE BUILD THIS PHASE: Reduce repetitive work while keeping judgment, sensitive actions and external commitments under human control.

## P06.06.1 Customer status agent

Coding-agent build instruction: Answer only using authorised case data and reviewed knowledge; show source/version, escalate uncertainty or complaint.

Technical implementation: Tool allowlist per agent, schema-validated outputs, source-grounding, prompt-injection defenses, PII masking, scoped retrieval, cost/rate limits and kill switch.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P06.06.2 Onboarding agent

Coding-agent build instruction: Explain checklist, classify uploads, extract fields into draft records; human verifies identity and compliance outcomes.

Technical implementation: Tool allowlist per agent, schema-validated outputs, source-grounding, prompt-injection defenses, PII masking, scoped retrieval, cost/rate limits and kill switch.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P06.06.3 Renewal agent

Coding-agent build instruction: Create reminders and draft outreach from verified expiry dates; respect preferences, template approvals and human escalation.

Technical implementation: Tool allowlist per agent, schema-validated outputs, source-grounding, prompt-injection defenses, PII masking, scoped retrieval, cost/rate limits and kill switch.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P07 Customer communication and controlled visibility

WHY WE BUILD THIS PHASE: Give customers reliable progress information without claiming government work is complete prematurely.

## P07.07.1 Messaging

Coding-agent build instruction: Integrate official WhatsApp provider or email behind adapter, consent/template control and message logs.

Technical implementation: Messaging adapter with consent and template status, webhook signature verification, delivery retries and idempotency; read-only status endpoint only if gate passed.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P07.07.2 Status view

Coding-agent build instruction: Provide secure minimal case-status page only when tested demand and budget gate approve; otherwise verified email/WhatsApp updates.

Technical implementation: Messaging adapter with consent and template status, webhook signature verification, delivery retries and idempotency; read-only status endpoint only if gate passed.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P07.07.3 Notifications

Coding-agent build instruction: Send threshold-based SLA alerts, missing-document requests and verified completion notices with deduplication.

Technical implementation: Messaging adapter with consent and template status, webhook signature verification, delivery retries and idempotency; read-only status endpoint only if gate passed.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P08 Management metrics and audit

WHY WE BUILD THIS PHASE: Measure actual service quality, customer outcomes, agent errors and unit economics from recorded events.

## P08.08.1 Event-derived KPIs

Coding-agent build instruction: Define formulas, numerator/denominator, exclusions, owner, cadence and data lineage for key metrics.

Technical implementation: Use event-time definitions and snapshot metric version; no unsecured raw SQL dashboard; audit export with retention and integrity checks.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P08.08.2 Dashboards

Coding-agent build instruction: Ship role-scoped operational dashboard then founder view; do not expose individual personal documents in analytics.

Technical implementation: Use event-time definitions and snapshot metric version; no unsecured raw SQL dashboard; audit export with retention and integrity checks.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P08.08.3 Audit and reconciliation

Coding-agent build instruction: Produce tamper-evident event chain/export, approval register, reconciliation exception queue and evidence archive.

Technical implementation: Use event-time definitions and snapshot metric version; no unsecured raw SQL dashboard; audit export with retention and integrity checks.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P09 Enterprise assurance and release

WHY WE BUILD THIS PHASE: Demonstrate the system is secure, reliable and recoverable before real customers depend on it.

## P09.09.1 Security verification

Coding-agent build instruction: Threat model and map OWASP ASVS 5.0.0 Level 2 target controls, access and agent abuse tests; independent review.

Technical implementation: Produce automated evidence for ASVS control mapping, OWASP ZAP safe test, backup restoration and dependency/security scans; staging-only preapproval.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P09.09.2 Reliability

Coding-agent build instruction: Verify backup restore, incident response, monitoring, rate limiting, migration rollback and disaster-recovery drill.

Technical implementation: Produce automated evidence for ASVS control mapping, OWASP ZAP safe test, backup restoration and dependency/security scans; staging-only preapproval.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P09.09.3 Release sign-off

Coding-agent build instruction: Run full E2E and regression with synthetic data, production checklist, manual UAT and documented approvals.

Technical implementation: Produce automated evidence for ASVS control mapping, OWASP ZAP safe test, backup restoration and dependency/security scans; staging-only preapproval.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# P10 Pilot, learn and expand

WHY WE BUILD THIS PHASE: Validate workflow and economics on actual cases before increasing automation or service coverage.

## P10.10.1 Controlled pilot

Coding-agent build instruction: Onboard limited approved customers, time every handoff, record issue and interruption and reconcile every case.

Technical implementation: Feature flags, limit pilot tenants, telemetry excluding PII, issue triage and rollback triggers; evidence-based expansion decision.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P10.10.2 Evidence-based improvements

Coding-agent build instruction: Prioritize backlog using missed SLAs, rework, documented customer requests and privacy/security risks.

Technical implementation: Feature flags, limit pilot tenants, telemetry excluding PII, issue triage and rollback triggers; evidence-based expansion decision.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

## P10.10.3 Expansion gate

Coding-agent build instruction: Consider portal, more agents, services and jurisdictions only on founder/compliance sign-off and proven unit economics.

Technical implementation: Feature flags, limit pilot tenants, telemetry excluding PII, issue triage and rollback triggers; evidence-based expansion decision.

Acceptance tests: happy path + invalid input + access denied + cross-tenant access + retry/duplicate + failure/recovery; demonstrate proof in PR, including phase-specific workflow and regression evidence.

EXIT GATE: All small-task acceptance criteria, security checks, documentation and UAT pass; named human reviewer signs phase; no unresolved critical/high security finding.

# 08 \| Locked technical baseline (proposed, not purchased)

| Layer                     | Default                                                                               | Rationale / decision guard                                                    |
|---------------------------|---------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| Language                  | TypeScript throughout first release; SQL migrations                                   | One type system; add Python service only if OCR/ML benchmark proves necessary |
| Web                       | Next.js current supported LTS-compatible version + accessible UI                      | Marketing site, minimal secure staff UI; strict server-side checks            |
| Backend                   | TypeScript API (NestJS or modular Node service; choose one via ADR)                   | Explicit validation and authorization; avoid two backends without need        |
| Database                  | Managed PostgreSQL with audited tenant controls                                       | Transactions, constraints, backups, strong relational case record             |
| Identity                  | Managed OIDC auth with MFA, enterprise SSO later                                      | No home-built authentication; scoped tokens                                   |
| Files                     | Encrypted private object storage, malware scan and expiring URLs                      | Never store passport images in Git, public buckets or logs                    |
| Jobs / workflow           | Postgres-backed outbox + worker and explicit case-state machine                       | Small scale first; Temporal only if reliability needs justify                 |
| CRM, finance and payments | Bought services behind versioned adapters                                             | Do not recreate regulated / commodity systems                                 |
| AI                        | Provider abstraction; deterministic pricing/rules; three bounded agents               | Model is not source of truth or statutory approver                            |
| Infra / ops               | UAE-region candidate after vendor/legal assessment; IaC, isolated environments, CI/CD | Location/transfer decision documented; secrets in manager                     |

Pin exact versions at project start after current license, maintenance and vulnerability verification. The two feasibility studies disagreed on GitHub API evidence: no dependency is approved solely because a repository has stars or recent commits. Save LICENSE, upstream URL, release, advisory result, test evidence and ADR. Avoid licensing-incompatible or unmaintained packages.

# 09 \| Concrete data and API contract

- Tables: tenants, users, memberships, roles, customers, contacts, services, service_versions, fee_versions, quotes, quote_lines, consent_records, cases, tasks, documents, document_reviews, approvals, external_submissions, receipts, invoices, payments_references, expiry_events, messages, agent_runs, audit_events.

- Every tenant-owned table has tenant_id; FK, uniqueness and database policy enforce tenant isolation. Record actor_id and actor_type; timestamps in UTC; show Dubai local time in UI. No mutable overwrite of approved fee/quote or audit events.

- Case states: DRAFT → QUOTED → ENGAGED → COMPLIANCE_PENDING → READY → HUMAN_SUBMITTED → AUTHORITY_PENDING → COMPLETED or REJECTED; PAUSED, CANCELLED, ESCALATED explicitly controlled. Prevent skipping required gates.

- API example routes: POST /leads, POST /quotes, POST /cases, GET /cases/:id, POST /cases/:id/transitions, POST /documents/upload-intent, POST /approvals/:id/decision, POST /webhooks/provider. Routes require authentication, tenant policy, validation, rate limits and audit.

- Financial invariant: quote totals = sum itemized lines under approved tax configuration; receipts matched to case and payment; refund never executed by AI; government charge never silently relabelled as agency revenue.

- External integration failure: queue durable retry with exponential backoff, idempotency key, dead-letter/manual replay and monitoring; never duplicate charge, official submission or outbound message.

# 10 \| Mandatory security engineering policy (all phases)

- Security target: OWASP ASVS 5.0.0 Level 2 as a verification baseline, with control-by-control applicability and evidence; supplement with OWASP API, LLM and agent threat models. ASVS mapping is not a certification.

- Identity: MFA on all staff/admin; SSO when ready; least-privilege RBAC plus tenant enforcement; emergency access time-bound and audited; service identities scoped separately from human accounts.

- App: output encoding, parameterized database access, strict schema validation, CSRF where applicable, secure cookies, rate limits, CSP, SSRF controls, secure uploads and webhooks, request size caps and no detailed error leakage.

- Data: TLS, managed encryption at rest, secrets manager and key rotation, document malware scanning, redacted logs, privacy processing inventory, documented retention/legal-hold policy, tested deletion/export, external LLM data-processing and transfer review.

- Agent: prompt injection is untrusted content; segregate system instructions from documents, tool allowlists, no direct SQL/system shell/government access, bounded context/tokens/spend, output validation, human approvals, run logging and per-agent off switch.

- Supply chain: lockfiles, SBOM, dependency review, license scan, SAST, secret scanning/push protection when plan supports, container/IaC scan, provenance/attestations as practical, vulnerability handling and patches.

- Availability: separate dev/staging/prod, backups with encrypted offsite copy, restore tests, incident contacts, monitored queues, documented recovery targets approved by founder, deployment rollback and audited migration procedure.

# 11 \| GitHub main-branch protections and PR protocol

- Private repository, founder retains organization ownership, MFA required and minimal developer permissions; protect main with an ACTIVE ruleset, prevent deletions and force-pushes, prohibit direct pushes including by coding bots.

- Only short-lived feature branches to pull requests; at least one independent human approval, CODEOWNERS approval for security/auth/finance/infrastructure, dismiss stale approvals, resolve conversations and require passing checks. More review for sensitive code as staffed.

- Require successful checks: formatting/lint, TypeScript typecheck, unit, integration, E2E smoke, coverage gate on changed code, dependency/secret/SAST/IaC scan, build and migration check. Require up-to-date merge base or merge queue.

- Do not give coding agent admin/bypass rights; no self-approving PR, no merging with failing checks, no production secret in CI logs. Required checks and scanning features depend on GitHub plan: equivalent external CI gates must be documented where unavailable.

- Each PR template must contain requirement ID, intent, exact files, screenshots, migration, threat assessment, tests with commands/results, roll-forward/rollback, docs update, cost changes and human review.

- Release from protected main only after staged deployment, migration dry run, independent sign-off and founder production approval. Use environment protection and credentials with minimal scope.

# 12 \| Test strategy and absolute definition of done

| Test level / gate    | Every change must prove                                                                                                                |
|----------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| Unit                 | Pure rules, calculations, pricing, state transitions and validation including negative/edge cases                                      |
| Integration          | PostgreSQL constraints, identity, queues, payment/CRM provider stubs and transaction atomicity                                         |
| End to end           | Browser-based journeys: lead→quote→approval→case→human submission record→completion; failure and recovery                              |
| Security             | Unauthorized role, cross-tenant, IDOR, file access, upload malware simulation, injection, prompt injection, rate limiting, PII leakage |
| Regression           | Run existing core journeys for every PR; add E2E for every user-visible feature or changed critical flow                               |
| Accessibility and UX | Keyboard, readable messages, mobile viewport, basic WCAG 2.2 AA evaluation and founder walkthrough                                     |
| Operational          | Backup-restore evidence, webhook replay, failed queue, monitoring alert, deploy/rollback, migration test                               |

Definition of Done for every feature: requirement linked; design/permissions reviewed; tests written and actually executed; no failing required check; no unresolved critical/high vulnerability; audit/security/privacy impact assessed; API/schema/runbook/end-user docs updated; staging demo and founder-readable summary attached; independent reviewer approves; PR merges to main; release only after separate gate. Never write “tested” without command, date and result; record blocked tests honestly.

# 13 \| File structure and coding-agent task packet

Suggested repository: apps/web, apps/api, packages/contracts, packages/ui, packages/config, infra, db/migrations, tests/unit, tests/integration, tests/e2e, docs/adr, docs/requirements, docs/security, docs/runbooks, docs/user-guides, .github/workflows and .github/PULL_REQUEST_TEMPLATE.md. Keep documents BRD-v0.1 and PRD-v0.1 in docs/requirements and link IDs to issue tracker.

Template for every ticket: ID; WHY (one sentence); business result; scope and exclusions; dependencies; exact screen/API/schema; user roles and agent permissions; test cases (happy/negative/cross-tenant/retry); logs/metrics; documentation; acceptance; estimated effort and extra cost; human approval. Break tickets to one independently testable outcome, preferably one small PR; do not group an entire phase into a single coding request.

# 14 \| Sample fully specified vertical slice: P04.03

| Field           | Requirement                                                                                                                                         |
|-----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| User story      | As an operations coordinator, I can transition a case to READY only after all required human checks are approved.                                   |
| Preconditions   | Authenticated staff tenant member, case in COMPLIANCE_PENDING, approved checklist and compliance sign-off.                                          |
| Implementation  | POST /cases/:id/transitions with target READY, expected case version and idempotency key; transactional policy check; append event.                 |
| Success         | State changes once, audit event created, assigned owner notified; customer sees only approved public status.                                        |
| Failure         | Missing approval =\> 409/422, wrong tenant =\> 404/403 per anti-enumeration design, duplicate key =\> same outcome, concurrent update =\> conflict. |
| Automated proof | Unit transition table, DB race/tenant integration tests, UI E2E permitted and denied user paths, queue replay test.                                 |
| Docs / reviewer | Update state map + API schema + runbook; operations lead and independent reviewer approve PR.                                                       |

# 15 \| Documentation deliverable registry

| Document / file                                                     | Created or updated when                                                |
|---------------------------------------------------------------------|------------------------------------------------------------------------|
| README / quickstart / glossary                                      | P01; update for every developer-facing change                          |
| BRD/PRD traceability and change log                                 | Every requirement edit; old decisions preserved                        |
| ADR / vendor and license register                                   | Each material architecture or dependency choice                        |
| Data dictionary / ERD / migration guide                             | Each schema modification                                               |
| OpenAPI schemas / integration contracts                             | Each API or webhook change                                             |
| Threat model / ASVS control matrix / privacy inventory              | P02 and every sensitive feature                                        |
| Agent cards, prompts, model/version register and evaluation sets    | P06 and each agent behavior change                                     |
| Test plan / CI evidence / known limitations                         | Every PR and release                                                   |
| Runbooks: incident, backup/restore, release, rollback, key rotation | Before production; review after changes                                |
| SOPs and founder guide with screenshots                             | Each operations-facing functionality; must be understandable to novice |

# 16 \| Production checklist, release criteria and handover

- Compliance and provider agreements signed, real-data use approved, privacy and retention notices reviewed; written government-channel mapping exists.

- Independent reviewer signs main PRs and final security evaluation. All critical/high findings fixed or release blocked. Pen-test scope and third-party review appropriate to risk before scaling.

- Migration rehearsed, backup restored, real-time alerts verified, load test against agreed pilot volume, RTO/RPO measured and approved, access/secret inventory signed.

- Founder sees demo in plain English; UAT scripts pass with synthetic data and approved pilot; price, source, receipt and account reconciliation checks pass.

- Prepare operational SOP, access offboarding, support contact, incident hotline, customer complaint and data-request process; approve rollback plan.

- Only then enable limited production; do not claim enterprise certification or regulatory compliance solely because software tests pass.

# 17 \| Decisions still required

Technical defaults are proposals. Select paid providers after privacy, UAE-region availability, subprocessors, licenses, cost and service-level review. Select LLM/OCR on representative redacted documents and measured false accepts, not marketing claims. Set concrete capacity, performance, retention, RTO/RPO and numeric acceptance thresholds using pilot evidence. Until then mark configuration PENDING and block production.

# References and provenance

\[S1\] Consolidated report A: Pasted markdown.md, 16 Sep 2026; internal study, assumptions not independently re-verified for this document.

\[S2\] Consolidated report B: Pasted markdown(1).md, 16 Sep 2026; internal study and documented limitations, not legal sign-off.

\[S3\] OWASP ASVS 5.0.0: https://owasp.org/www-project-application-security-verification-standard/ ; stable baseline, accessed 16 Sep 2026.

\[S4\] GitHub rulesets: https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/available-rules-for-rulesets ; actual functionality varies by plan.

\[S5\] GitHub PR governance: https://docs.github.com/en/pull-requests/reference/managing-and-standardizing-pull-requests ; templates, CODEOWNERS, protected branches.

\[S6\] UAE authority sources: Obtain dated official DET, MOHRE, GDRFA, ICP, FTA, Ministry and data-protection guidance and written professional advice before enabling regulated flows; exact rules not certified here.

This document distinguishes research claims from confirmed production requirements. It is not a legal opinion, independent penetration-test report or confirmed vendor procurement estimate.
