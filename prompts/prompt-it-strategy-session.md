I'm working on a proposal to outline and summarise an IT strategy for Bupa (a multi-national healthcare and insurance company) in a single page.

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
- Specific things we would like to see accounted for:
  - Single view of health
  - Portable cloud-ready
  - Single customer view
  - Interoperability - APIs and data
  - Standardise on protocols (contracts) not products
  - Service layer that abstracts underlying fulfilment business
  - Platforms that make delivery safe, fast, and efficient by default.

Create the proposal as a new Markdown file. Ask me for guidance and feedback where appropriate.

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
