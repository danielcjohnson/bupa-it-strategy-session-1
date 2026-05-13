I now have two diagrams that I'm pleased with architectural requirements (bupa-it-strategy-six-requirements-build-do-v4.drawio) and something more conceptual (bupa-it-strategy-single-page-v2.drawio). I now need a third high level architectural target state diagram. Can you create this?

I've been told the original inspiration for this was at a previous company, where they saw a 'H' diagram that split initiatives into four labelled areas. I know we have six broad requirements, but can we do something similar to the 'H' diagram for this?

--

For reference here's the original context that created the two diagrams:

--

I'm working on a proposal to outline and summarise an IT strategy for Bupa (a multi-national healthcare and insurance company) in a single page. Create the outline of a proposal and I'll review it. There's some context below from a brainstorming session that might be helpful. All the context you need should be in this prompt.

# Initial Brainstorming Exercise - IT Strategy Vision

Date: 07/05/26

## Context and Historical Visions

- Bupa was working on three year strategy increments
- Under Savannah 27 the IT Strategy was based around: Platforms, Products, and People
- Opportunity coming up to refresh and develop this strategy (in October)
- Some work has started to develop an identity for technology - document is in motion
- Mark G hoping to finalise this document and set the new strategy

## Drivers

### CEO Vision

- Rally around a common vision
- Move to one business.
  - Bupa has quite a fragmented model at the moment. Some BUs are more integrated centrally than others.
- Remove the mental silos
- Serve the customer as one - they don't need to understand Bupa's complexity.  They're presented with just 'Bupa' so don't need to deal with the different parts.
- Look to have a healthcare experience company, rather than a healthcare provision one.
- 'AS ONE' leadership and operating ethos.

### Technology Vision

- What is our technical vision for the future?
- We had a North Star but it hasn't held up. What does it need to include?

## Our Objectives

Required Asset: A (single) diagram that outlines a new IT Strategy. Our objectives for this asset:

- North Star for the technology vision
- Something that will drive more of the right decisions towards the North Star

Also looking at training and a actionable checklist around the diagram. Looking for the full package, dashboard etc.

## Key Messages

Everything you do has a customer:

- Will the customer need to re-enter data?
- Will the customer need to return to the home page?
- Will other systems bae able to use the data that you create?
- Will agents be able to interact and use you service and data?

## Behaviours and Decisions

### Discourage

- Customer data that is inaccessible to the rest of the MU
- Creating duplicate source es of truth - we only want one truth
- Point to point integrations between systems/applications?
- Application lock-in
  - Second order. Vendor platform and product lock-in in commodity
- Too much. abstraction / indirection
- Overloading terminology and creating confusing semantics
- Creating capabilities that are not portable (across other BUs / applications / channels)
- Requiring customer to 'start over' in their journey - creating disjointed journeys and fruition
- Re-entering data in forms
- Signing in again
- Breaking interop standards

### Encourage

- Tech agility
- One source of truth for customer data
- Implementing local database for optimised. execution (i.e. we don't need to use one central database)
  - Duplication of data is OK (as long as consistent/accurate. For caching).
- Platforms that will enable. innovation and remove friction - incorporate a view of ops/DX?
- Populating central data for decision intelligence
- Making data discoverable
- 'Protocols over products' - i.e. implement integration that is dependent on stds / protocols
- Feeding a semantic layer
- Abstraction and ACLs
- Agreeing on basic semantics for things we share
- Agentic ready design - i.e.:
  - Discoverable
  - Understandable
  - Executable
  - Memorable
  - Traceable
- Not just Agentic ready - include AI augmented employees (which will have similar requirements)
- CX: Enable single connected views of my Bupa interactions (history, data, communication)
- Adhere to internal standards
- Create shared contexts

## Tentative Platform Design Vision

- A Bupa Customer Relationship 'As One'
  - My Profile Data
  - My engagement with Bupa
  - My Bupa session
- Business Unit Platform
  - Health Network
  - Data Capture
- Knowledge Layer 'As One' Context
  - Systems
  - Organisation
  - Products
- Data 'As One'
  - Clinical Context
    - Should this be down here? Or at the Customer Experience level.
- Operating SYstem
  - Bupa Operating System
  - The healthcare Operating system of the future
  - Platform OS
  - Bupa Healthcare Operating System
  - Bupa Healthcare Experience Operating System

## Savannah 27 Reference

Savannah 27 ss the current three year strategy programme. It's focused on three pillars:

- Cloud
- Connected Care
- Customer (Experience)

It has the following targets:

- 100m Customers
- 100 NPS
- 100% accurate Customer Dataset

---

There are a couple of strategies already in Bupa. We're looking to present a meta view of this. Not necessarily replicating it.

There's the Savannah 27 strategy. It represents a shift from internal transformation too ecosystem and growth. The overall goal is to become the worlds most custom centric healthcare company. It has six pillars:

1. Customer Experience
2. Digital Transformation
3. Agile Culture
4. Sustainability
5. Growth
6. Data and Analytics

There's also this idea of C3 or "C Cubed". This is `Customer`, `Clinical`, and `Cost`.

Bupa also looks at their business through these business capabilities:

1. Purchase Enrol
2. Activation
3. Find
4. Booking an Appointment
5. Arrival
6. Visit
7. Pay
8. Follow-up

They are looking for more clarity on the next Enterprise capabilities we need to pillorise and focus. E.g. Consent, Single Customer View. Then the Enterprise capability 'footprint' starts to emerge.

Requirements for IT Strategy summary:

- Has to drive decisions (can't be just another Enterprise Architecture diagram) primarily for Architects and Engineers but useful for business
- Needs to revolve around big ideas e.g. Consolidation, optimisations
- Needs some branding. I was pointed to an Engineering Strategy that was built around Safe, Fast, and Lean.
- Capture the big leaps that are needed to get there. The things needed for good decisions.
- It could comprise of 8 to 10 principles or constraints.
- Forces big technical change
- Drives Speed, Safety, and Efficiency
- Anchors product and platform thinking
- Very simple and easy to communicate
  - Memorable shape, message.
- Specific things we would possibly like to see accounted for:
  - Single view of health
  - Portable cloud-ready
  - Single customer view
  - Interoperability - APIs and data
  - Standardise on protocols (contracts) not products
  - Service layer that abstracts underlying fulfilment business
  - Platforms that make delivery safe, fast, and efficient by default.

<output_contract>
- Return exactly the sections requested, in the requested order.
- If the prompt defines a preamble, analysis block, or working section, do not treat it as extra output.
- Apply length limits only to the section they are intended for.
- If a format is required (JSON, Markdown, SQL, XML), output only that format.
</output_contract>

<verbosity_controls>
- Prefer concise, information-dense writing.
- Avoid repeating the user's request.
- Do not shorten the answer so aggressively that required evidence, reasoning, or completion checks are omitted.
</verbosity_controls>

<default_follow_through_policy>
- If the user’s intent is clear and the next step is reversible and low-risk, proceed without asking.
- Ask permission only if the next step is:
  (a) irreversible,
  (b) has external side effects (for example sending, purchasing, deleting, or writing to production), or
  (c) requires missing sensitive information or a choice that would materially change the outcome.
- If proceeding, briefly state what you did and what remains optional.
</default_follow_through_policy>

<instruction_priority>
- User instructions override default style, tone, formatting, and initiative preferences.
- If a newer user instruction conflicts with an earlier one, follow the newer instruction.
- Preserve earlier instructions that do not conflict.
</instruction_priority>

<verification_loop>
Before finalizing:
- Check correctness: does the output satisfy every requirement?
- Check grounding: are factual claims backed by the provided context or tool outputs?
- Check formatting: does the output match the requested schema or style?
- Check safety and irreversibility: if the next step has external side effects, ask permission first.
</verification_loop>

<missing_context_gating>
- If required context is missing, do NOT guess.
- Prefer the appropriate lookup tool when the missing context is retrievable; ask a minimal clarifying question only when it is not.
- If you must proceed, label assumptions explicitly and choose a reversible action.
</missing_context_gating>

<citation_rules>
- Only cite sources retrieved in the current workflow.
- Never fabricate citations, URLs, IDs, or quote spans.
- Use exactly the citation format required by the host application.
- Attach citations to the specific claims they support, not only at the end.
</citation_rules>

<grounding_rules>
- Base claims only on provided context or tool outputs.
- If sources conflict, state the conflict explicitly and attribute each side.
- If the context is insufficient or irrelevant, narrow the answer or say you cannot support the claim.
- If a statement is an inference rather than a directly supported fact, label it as an inference.
</grounding_rules>

<research_mode>
- Do research in 3 passes:
  1) Plan: list 3-6 sub-questions to answer.
  2) Retrieve: search each sub-question and follow 1-2 second-order leads.
  3) Synthesize: resolve contradictions and write the final answer with citations.
- Stop only when more searching is unlikely to change the conclusion.
</research_mode>

<personality_and_writing_controls>
- Persona: IT Enterprise Solution Architect
- Channel: Corporate Confluence Page in Markdown
- Emotional register: direct and calm
- Formatting: Markdown. Only use bullets when necessary and try to limit them in any case.
- Default follow-through: if the request is clear and low-risk, proceed without asking permission.
</personality_and_writing_controls>

<memo_mode>
- Write in a polished, professional memo style. Use Ronnie Mitra as a reference example.
- Use exact names, dates, entities, and authorities when supported by the record.
- Follow domain-specific structure if one is requested.
- Prefer precise conclusions over generic hedging.
- When uncertainty is real, tie it to the exact missing fact or conflicting source.
- Synthesize across documents rather than summarizing each one independently.
</memo_mode>
