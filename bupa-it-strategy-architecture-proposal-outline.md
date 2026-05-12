# Bupa IT Strategy Proposal: Architectural North Star

**Date:** 11/05/26
**Status:** Proposal draft
**Audience:** Technology leadership, enterprise architects, solution architects, engineers, platform teams, product leaders, and business sponsors

## 1. Executive Position

Bupa needs a technology North Star that is more than a conceptual strategy picture. It should show the architectural things Bupa must build, the delivery moves Bupa must make, and the decision rules that should change day-to-day engineering choices.

The proposed position is:

> **Build Bupa's connected healthcare experience platform: shared customer and health context, reusable enterprise services, contract-led interoperability, governed data, and paved roads for delivery.**

This is the architectural route to the **As One** ambition. Customers should experience Bupa as one organisation. Business units can still differentiate in service model and fulfilment, but they should do so behind common contracts, shared semantics, and reusable platform capabilities.

## 2. What Changed From the Previous Diagram

The earlier diagram framed the strategy well, but it read as an operating concept. The next version should be more explicit about what must exist in the target architecture.

The new diagram should therefore show:

| From | To |
| --- | --- |
| Context-ready as a broad concept | A concrete architecture made of context services, capability services, interoperability, data products, and developer platforms |
| Principles around the centre | Six architectural requirements that act as design tests |
| Platform as an abstract enabler | Developer platform as a visible product with golden paths, controls, observability, and Time to HelloWorld |
| Business unit complexity shown as context | Business unit fulfilment explicitly abstracted behind service contracts and adapters |
| AI and agents as a future consideration | Human, system, and authorised AI consumption designed into services, data, and knowledge from the start |

## 3. North Star

**Bupa As One Technology North Star**

Bupa should build a connected healthcare experience platform that lets customers, colleagues, clinicians, partners, systems, and authorised AI agents operate with shared, governed context.

The practical test is simple:

> A customer should not have to restart, a team should not have to rediscover the enterprise, and a system should not have to integrate through bespoke point-to-point plumbing.

This is not a call for one global application or one physical database. It is a call for one coherent architectural model: common contracts, authoritative sources of truth, governed copies, reusable enterprise capabilities, and delivery paths that make the right thing easier than the local workaround.

## 4. Six Architectural Requirements

The 'six requirements' should be treated as a communication device rather than a strict count from the source material. These are the distilled design tests from the behaviours and decisions feedback.

| Requirement | Architectural Test | Build Implication |
| --- | --- | --- |
| **1. Single customer and health context** | Can the journey continue without the customer re-entering data, signing in again, or returning to the start? | Build shared identity, profile, session, consent, interaction, and health context services. |
| **2. One truth, many governed copies** | Is there a named source of truth, with local copies allowed only where lineage, consistency, and ownership are clear? | Build authoritative data ownership, local cache rules, synchronisation patterns, quality controls, and lineage. |
| **3. Contracts and protocols before products** | Is the integration based on stable APIs, events, data contracts, and health interoperability standards rather than product coupling? | Build an API, event, and data contract platform with OpenAPI, AsyncAPI, FHIR-aligned patterns, versioning, and conformance checks. |
| **4. Shared capability services before local rebuild** | Is the team reusing or extending an enterprise capability before creating another local implementation? | Build service layers for consent, eligibility, booking, payment, claims, provider, communication, care navigation, and orchestration. |
| **5. Context-ready data and knowledge** | Can people, systems, and authorised AI agents discover, understand, execute, and trace the service or data asset? | Build catalogues, semantic models, metadata, examples, policy evidence, runbooks, and machine-consumable service descriptions. |
| **6. Paved roads for developers and operators** | Can a team create, secure, deploy, observe, and integrate a Bupa-standard service quickly through the preferred path? | Build a developer portal, golden paths, templates, CI/CD, environments, policy as code, observability, operational readiness, and cost controls. |

## 5. What Bupa Needs to Build

The target architecture should be described as a small set of enterprise build components.

| Build Component | Purpose | Examples |
| --- | --- | --- |
| **Experience and composition layer** | Connect journeys across channels, products, markets, and business units without exposing internal complexity. | Journey orchestration, channel APIs, session continuity, customer interaction history, colleague and clinician workflow composition. |
| **Bupa relationship context** | Provide the reusable context required for a customer, member, patient, provider, colleague, or authorised agent to act. | Identity, party model, profile, consent, preferences, session, engagement history, communication history, health context. |
| **Enterprise capability services** | Expose common business capabilities as reusable services rather than rebuilding them in each product or BU. | Eligibility, booking, provider search, referral, payment, claims, document exchange, care navigation, communication, follow-up. |
| **Contract-led interoperability fabric** | Replace point-to-point integrations with governed contracts, protocols, events, and adapters. | API gateway, event platform, contract registry, schema registry, FHIR-aligned exchange, service ACLs, partner adapters. |
| **Data and knowledge plane** | Turn operational activity into trusted context, decision intelligence, and reusable enterprise knowledge. | Data products, semantic layer, catalogue, lineage, quality scoring, decision intelligence, operational knowledge, clinical context. |
| **Developer platform and operating control plane** | Make secure, compliant, observable, efficient delivery the default path for teams. | Developer portal, golden paths, service templates, infrastructure as code, CI/CD, secrets, IAM, observability, SLOs, policy as code, FinOps. |

## 6. What Bupa Needs to Do

The diagram should make the work visible, not just the end state.

| Delivery Move | Why It Matters | First Action |
| --- | --- | --- |
| **Name accountable capability owners** | Shared capabilities will not converge without ownership, funding, roadmap authority, and lifecycle accountability. | Assign owners for customer context, consent, health context, interoperability, data products, and developer platform. |
| **Publish the contract and semantic catalogue** | Reuse depends on teams knowing what terms, APIs, events, and data products already exist. | Create an initial catalogue for customer, member, patient, provider, consent, appointment, product, policy, claim, interaction, and health context. |
| **Build the first golden paths** | Developer Experience has to become a platform product, not a documentation exercise. | Create a service golden path that gets from repository to deployed, secured, observable, documented service. |
| **Measure Time to HelloWorld** | Platform friction must be visible enough to improve. | Track elapsed time from approved team start to first Bupa-standard deployed service with security, observability, and a published contract. |
| **Migrate priority journeys through the service layer** | The architecture only matters if it improves real customer and colleague journeys. | Start with high-value journeys across purchase/enrol, activation, find, booking, visit, pay, and follow-up. |
| **Reduce point-to-point and duplicate truth by policy** | Local optimisation should not keep recreating enterprise complexity. | Introduce an exception model for new point-to-point integration, duplicate source of truth, non-portable capability, or unsupported platform path. |
| **Create the North Star dashboard** | Strategy adoption should be measured through decision behaviour and delivery outcomes. | Track Time to HelloWorld, contract reuse, API/event adoption, point-to-point reduction, journey restart rate, data quality, SLOs, and control evidence. |

## 7. Opinionated Decision Guardrails

The strategy should force choices. The proposed guardrails are:

1. **No new strategic integration without a contract.** APIs, events, data products, and clinical exchange patterns must be versioned, discoverable, and owned.
2. **No new duplicate source of truth without an explicit exception.** Local stores are acceptable for performance, resilience, and autonomy when lineage and consistency are governed.
3. **No customer journey should restart because Bupa systems cannot share context.** Identity, consent, profile, session, communication history, and health context must be reusable.
4. **No product or vendor should define the enterprise contract.** Products can implement capabilities, but Bupa owns the semantics, contracts, and portability requirements.
5. **No team should build common plumbing from scratch.** Security, deployment, observability, secrets, runtime, API publication, and operational readiness should come from platform golden paths.
6. **No local capability should become strategic by accident.** Capabilities that are reused across markets or journeys need ownership, funding, standards, lifecycle management, and adoption measures.
7. **No AI or automation without traceable context.** Services, data, policies, and actions must be discoverable, understandable, executable through governed interfaces, and auditable.
8. **No architecture exception without an owner and review date.** Divergence is allowed where it creates market, regulatory, or clinical value, but it should be deliberate.

## 8. Developer Experience and Time to HelloWorld

Developer Experience should be treated as a strategic capability because it determines whether architects and engineers follow the North Star in practice.

**Time to HelloWorld** should become the headline friction measure:

> How long does it take a team to create, secure, deploy, observe, document, and integrate a minimal Bupa-standard service through the preferred platform path?

The measure should include:

| Dimension | Minimum Expectation |
| --- | --- |
| **Create** | Service generated from an approved template with ownership and repository standards. |
| **Secure** | Identity, secrets, dependency checks, access controls, and baseline policy evidence in place. |
| **Deploy** | Automated pipeline to a supported environment using approved infrastructure patterns. |
| **Observe** | Logs, metrics, traces, health checks, SLO hooks, and alert routes available by default. |
| **Integrate** | API, event, or data contract published to the catalogue with examples and ownership. |
| **Operate** | Runbook, support route, cost visibility, resilience expectations, and lifecycle status visible. |
| **Context-ready** | Metadata, semantics, usage constraints, and audit trail clear enough for people, systems, and authorised AI agents. |

The goal is not a faster prototype. The goal is a faster compliant path to real delivery.

## 9. Diagram Narrative

The revised draw.io diagram uses this structure:

1. **North Star at the top:** connected healthcare experience platform for Bupa As One.
2. **Journey demand below it:** customer and colleague journeys that need continuity.
3. **Architectural build components in the centre:** experience composition, relationship context, enterprise capability services, contract-led interoperability, data and knowledge, business unit fulfilment adapters, and the developer platform.
4. **Six architectural requirements on the left:** the design tests that every strategic initiative should satisfy.
5. **Delivery moves and measures on the right:** the work required to make the architecture real.
6. **Opinionated guardrails at the bottom:** the decisions the strategy should make easier to say yes or no to.

This keeps the diagram architectural while still being usable as a single-page strategy asset.

## 10. Recommended Next Package

The single-page diagram should be supported by a small operating pack:

| Artefact | Purpose |
| --- | --- |
| **Architecture decision checklist** | Turns the six requirements into review questions for architects and engineers. |
| **Capability ownership map** | Names the owner, roadmap, standards, current platforms, and convergence path for each enterprise capability. |
| **Contract and semantic catalogue starter** | Creates the first reusable vocabulary and integration inventory. |
| **Developer golden path backlog** | Prioritises improvements that reduce Time to HelloWorld. |
| **North Star dashboard** | Shows whether decisions are moving towards reuse, interoperability, journey continuity, safety, speed, and efficiency. |
