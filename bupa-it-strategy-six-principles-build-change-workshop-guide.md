# Six Principles Build and Change Workshop Guide

## 1. Single Customer and Health Context

Intent: Bupa recognises the customer across journeys, so customers do not restart, re-key, or repeat themselves.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| Bupa Customer Relationship As One | Create funded owners for reusable customer context services | Treat customer context as a reusable product, with ownership and funding beyond a single journey. |
| My profile data | Stop duplicate capture in new builds | If a profile attribute already exists, new initiatives should consume it rather than ask again. |
| My engagement with Bupa | Route priority journeys through shared context | Use previous interactions and journey history to make the next step feel connected. |
| My Bupa session | Route priority journeys through shared context | Preserve session and hand-off context where a customer moves between channels or services. |
| My health context | Name context owners | Make ownership explicit for sensitive health context so it can be reused safely and consistently. |

**Standalone / cross-cutting:** `Name context owners` also applies across profile, engagement, session, and health context. Use it as a governance question whenever participants propose a new shared context item.

## 2. Single Source of Truth, Governed Copies

Intent: Bupa gives consistent answers, even where data is cached, copied, or used locally.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| Data ownership register | Assign data owners and stewards | Start with clear accountability: who owns the data, who stewards it, and who decides exceptions? |
| Authoritative data products | Require exceptions for duplicate truth | Make the authoritative source explicit, then require review when a local source claims to be another truth. |
| Governed local stores and caches | Define freshness and reconciliation rules | Local copies are acceptable when the rules for staleness, refresh, and reconciliation are clear. |
| Event propagation and reconciliation | Define freshness and reconciliation rules | Events should not just move data; they should support traceable correction and alignment. |
| Lineage, quality and freshness controls | Measure accuracy, completeness and reuse | Controls need visible measures, otherwise teams cannot tell whether trust is improving. |

**Standalone / cross-cutting:** `Measure accuracy, completeness and reuse` can be used as a common scorecard across all data initiatives, not only lineage and quality controls.

## 3. Standardise on Protocols, not Products

Intent: Bupa systems connect through shared standards and portable patterns, not vendor lock-in. FHIR adoption is a strong example because Bupa is already committed to developing it further.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| FHIR-aligned clinical exchange patterns | Publish examples and lifecycle rules | Make FHIR practical by giving teams examples, version guidance, and rules for evolving the pattern. |
| OpenAPI and AsyncAPI standards | Version interface specifications and test conformance | Standards only help if teams can check whether APIs and events actually conform to them. |
| API, event and data interface registry | Include standards and interoperability review before funding | Use review to test portability and protocol fit before teams commit to a solution path. |
| Gateway, event bus and schema registry | Contain unmanaged point-to-point integration | Provide supported integration routes so teams do not need to create bespoke connections by default. |
| Partner and BU adapter patterns | Publish examples and lifecycle rules | Make partner and BU variation explicit at the edge while keeping core protocols consistent. |

**Standalone / cross-cutting:** `Contain unmanaged point-to-point integration` should be handled carefully in the workshop. It is useful where point-to-point integration creates fragility, but it should not read as a blanket ban without context.

## 4. Shared Capability Services

Intent: Bupa can deliver one experience across different BU fulfilment models by reusing shared capabilities where they make sense.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| Consent, eligibility and entitlement services | Name capability owners and roadmaps | These capabilities need clear owners because they shape what customers are allowed or entitled to do. |
| Booking, provider, referral and care navigation | Migrate priority journeys incrementally | Start with the journeys where shared booking, referral, or navigation creates the most customer value. |
| Payment, claims and document exchange | Fund shared service lifecycle management | These services need product-style funding for reliability, change, and ongoing support. |
| Communication and follow-up services | Migrate priority journeys incrementally | Use follow-up as a visible customer improvement: fewer dropped hand-offs, clearer next steps. |
| BU adapters for Health Network and Data Capture | Retire or contain duplicate local capabilities | Use adapters to respect local fulfilment differences while reducing duplicated core capability. |

**Standalone / cross-cutting:** `Fund shared service lifecycle management` applies to every shared capability once it becomes relied upon by more than one journey or BU.

## 5. Knowledge Layer As One Context

Intent: People, systems, and authorised agents understand Bupa services through shared meaning, context, and machine-readable descriptions.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| Semantic layer and shared glossary | Agree shared meanings for key terms | Start with terms that create operational confusion across journeys, products, markets, or BUs. |
| Catalogue for systems, organisation and products | Make cataloguing part of delivery | Catalogue entries should be a delivery artefact, not a clean-up task after go-live. |
| Clinical, policy and journey context | Publish machine-consumable descriptions, including schemas | Important context should be usable by systems and authorised agents, not only documented for people. |
| Metadata, examples and usage constraints | Publish machine-consumable descriptions, including schemas | Pair metadata with examples and constraints so reuse is safe, not just technically possible. |
| Decision intelligence feeds | Design for authorised AI and employee augmentation | Treat decision feeds as governed inputs to colleague support, automation, and AI-assisted workflows. |

## 6. Developer Experience and Golden Paths

Intent: Teams can build joined-up services without rebuilding the basics or negotiating every delivery pattern from scratch.

| Build initiative | Related Change initiative | Workshop steer |
| --- | --- | --- |
| Developer desktop experience | Address Developer Desktop issues | Remove the day-to-day friction that stops teams from using the preferred paths. |
| Golden paths | Deliver priority golden paths on a lean foundation | Focus on the few golden paths that unlock priority initiatives first. |
| Service templates and infrastructure as code | Deliver priority golden paths on a lean foundation | Templates and IaC should be the concrete starting point for golden path adoption. |
| CI/CD, IAM, secrets and policy as code | Implement DX strategic target operating model | These controls need a clear operating model so teams know what is self-service and what is governed. |
| Observability, SLOs and runbooks | Implement DX strategic target operating model | Operational expectations should be part of the path, not added after launch. |
| Runtime, cloud and FinOps controls | Implement DX strategic target operating model | Give teams supported runtime and cost-control patterns so delivery speed does not create unmanaged risk. |

**Standalone / cross-cutting:** `Measure Time to HelloWorld end to end` is best used as a DX health metric across all developer experience initiatives, not as a single Build/Change pair.

## Quick Facilitation Questions

Use these when an initiative is being discussed:

1. Which principle does this initiative advance most directly?
2. What is the Build item that would make the principle real?
3. What Change item must happen for that Build item to be adopted, governed, or sustained?
4. Is this a reusable capability, a local journey improvement, or a cross-cutting enabler?
5. Who owns the next step, and what open question must be resolved before the initiative can move forward?
