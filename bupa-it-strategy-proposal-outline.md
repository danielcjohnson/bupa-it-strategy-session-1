# Bupa IT Strategy Proposal Outline

## 1. Working Title

**One Bupa Technology Strategy: Safe, Fast, Connected**

A meta-strategy for IT decisions that translates Bupa's customer-centric healthcare ambition into architecture, engineering, platform, and delivery choices.

## 2. Core Proposition

Bupa should organise its next phase of IT strategy around one idea:

**Create a governed connected health and care technology platform that gives Bupa trusted customer and health context, interoperable care and insurance services, and safe delivery paths by default.**

The purpose is to make customer, clinical, and cost outcomes easier to improve and measure across markets.

The strategy is not another enterprise architecture diagram. It is a decision framework for where to consolidate, where to standardise, where to abstract local complexity, where resilience and clinical safety must be mandatory, and where business units should continue to differentiate.

## 3. Strategic Shifts

| Strategic Shift | From | To | Decision It Drives |
| --- | --- | --- | --- |
| **1. From fragmented context to trusted context** | Customer, health, consent, product, and journey data held in separate systems | Shared, governed views of customer, health, consent, eligibility, and interaction history | Stop rebuilding identity, customer, and health context in every channel or business unit |
| **2. From point-to-point integration to enterprise interoperability** | Local integrations, product-specific APIs, duplicated data flows | Standard APIs, events, data contracts, clinical protocols, and interoperability patterns | Standardise on contracts and protocols before products |
| **3. From local delivery effort to platform-enabled delivery** | Teams repeatedly solving security, compliance, deployment, observability, resilience, and cloud foundations | Platforms that make safe, fast, resilient, efficient delivery the default path | Shift effort from repeated plumbing to product, care, and customer outcomes |

## 4. Priority Enterprise Capabilities

The first capability footprint should be small enough to govern and broad enough to change delivery behaviour.

| Capability | Enterprise Purpose |
| --- | --- |
| **Customer identity and party model** | Establish one trusted representation of customers, members, patients, brokers, providers, clinicians, and related parties. |
| **Consent and preferences** | Separate clinical consent, privacy permissions, marketing preferences, data-sharing permissions, and audit evidence. |
| **Customer context** | Provide reusable views of relationship, coverage, eligibility, product, interaction, and journey history. |
| **Health context** | Provide governed access to relevant health information, clinical context, care plans, observations, and care history. |
| **Eligibility, funding, claims, and billing services** | Abstract insurance and fulfilment complexity behind reusable service layers. |
| **Provider and partner connectivity** | Make referrals, appointments, directories, claims, documents, and data exchange easier to integrate across the ecosystem. |
| **API, event, and data contract platform** | Manage reusable service contracts, event schemas, data products, versioning, conformance, and lifecycle controls. |
| **Cloud and developer platform** | Provide golden paths for secure delivery, deployment, observability, recovery, cost management, and compliance. |
| **Clinical safety, AI, and evidence governance** | Ensure digital, data, automation, and AI-enabled services are clinically appropriate, auditable, and responsibly operated. |
| **Enterprise observability and value management** | Make reliability, adoption, journey performance, unit cost, safety, and value visible enough to manage. |

## 5. Decision Rights and Ownership

Each enterprise capability needs one accountable owner with authority over roadmap, funding, standards, adoption, lifecycle health, and value evidence.

| Decision Area | Default Decision Right |
| --- | --- |
| **Capability ownership** | Enterprise capability owner, with market and business unit representation. |
| **Architecture standards** | Enterprise architecture, platform, security, privacy, data, and clinical safety authorities. |
| **Product and platform roadmaps** | Capability owner and platform/product leadership, tied to funded outcomes. |
| **Local variation** | Market or business unit owner, approved through the exception model. |
| **Retirement and convergence** | Capability owner and investment governance, with explicit transition funding. |
| **Risk acceptance** | Named accountable executive, supported by security, privacy, resilience, and clinical safety evidence. |

## 6. Mandatory Standards and Constraints

The strategy should make a small set of standards mandatory wherever the relevant pattern applies.

| Standard or Constraint | Where It Applies |
| --- | --- |
| **Contracts before products** | New integrations, platform choices, data products, ecosystem services, and major procurements. |
| **FHIR-aligned clinical exchange** | Clinical and health data interoperability, where the use case involves health records, observations, care plans, eligibility, claims, consent, provenance, or audit events. |
| **OpenAPI and AsyncAPI contract governance** | Synchronous APIs, asynchronous events, partner interfaces, and internal service boundaries. |
| **Data product controls** | Critical customer, health, operational, and financial data used for decisions, AI, analytics, or reporting. |
| **Consent, privacy, and audit by design** | Customer, health, marketing, personalisation, AI, and ecosystem data-sharing use cases. |
| **Operational resilience by design** | Important business services, clinical workflows, customer journeys, payment/claims flows, and critical platform dependencies. |
| **Cloud-ready and portable architecture** | New services, material platform changes, and strategic vendor decisions. |
| **Platform golden paths** | Delivery pipelines, observability, security controls, deployment, recovery, and cost management. |

## 7. Proposed Principles

1. Customer, Clinical, Cost is the primary trade-off model.
2. One customer, many journeys.
3. One health view, governed by consent, privacy, clinical safety, and audit evidence.
4. Contracts before products.
5. Abstract fulfilment complexity behind service layers.
6. Cloud-ready and portable by design.
7. Platforms make the right path easy and the risky path visible.
8. Consolidate where Bupa needs leverage.
9. Differentiate where local market value matters.
10. Measure reuse, speed, safety, efficiency, and outcomes.

## 8. Outcome Scorecard

The strategy should be judged by whether it changes delivery behaviour and business outcomes, not by whether the target architecture is documented.

| Outcome | Example Measures |
| --- | --- |
| **Reuse** | Adoption of shared capabilities, API/event reuse, duplicated system retirement, percentage of journeys using enterprise context services. |
| **Speed** | Lead time for change, deployment frequency, onboarding time for new services or partners, time to launch market variation. |
| **Safety** | Clinical safety evidence, policy compliance, privacy incidents, security incidents, high-severity defects, resilience test outcomes. |
| **Efficiency** | Cost-to-serve, platform unit cost, operational effort removed, manual work reduced, integration run cost reduced. |
| **Customer and care outcomes** | Journey completion, digital containment where appropriate, NPS-linked journey improvements, care continuity, claims/payment friction. |
| **Data quality and trust** | Data product quality scores, lineage coverage, consent traceability, decision-grade dataset adoption. |

## 9. Exception Model

Local differentiation is allowed where it creates market value, responds to regulation, or protects a clinically necessary workflow. It should not be an unmanaged default.

Each exception should have:

1. A named owner.
2. The customer, clinical, cost, regulatory, or market reason for variation.
3. The cost and risk of divergence.
4. A review date or expiry condition.
5. A convergence, containment, or deliberate-local decision.

## 10. Updated One-Page Message

**One Bupa Technology Strategy: Safe, Fast, Connected**

To become the world's most customer-centric healthcare company, Bupa needs technology that can create trusted customer and health context, connect care safely, and deliver change quickly across markets.

The strategy is built around three strategic shifts:

1. From fragmented context to trusted context.
2. From point-to-point integration to enterprise interoperability.
3. From local delivery effort to platform-enabled delivery.

The rule is simple:

**Standardise the contracts. Consolidate the common capabilities. Differentiate the care and customer experience.**

The decision test is equally simple:

**If an initiative does not improve customer, clinical, or cost outcomes; reuse enterprise capabilities; and make delivery safer, faster, or more efficient, it should not be treated as strategic.**
