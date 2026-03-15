---
name: research-writing
description: |
  Produce informed, measured, evidence-driven long-form prose that reads as thoughtful and
  credible rather than promotional or AI-generated. Use this skill whenever the user asks you
  to write blog posts, research summaries, product announcements, technical narratives,
  industry analyses, white papers, thought leadership pieces, or any long-form content that
  should feel researched, authoritative, and human. Also trigger when the user says "make this
  sound informed," "research-style writing," "write a blog post," "draft an announcement,"
  "write this like a real person," or asks for writing that is "thoughtful," "measured," or
  "credible." Trigger even when the user doesn't explicitly name this style but clearly wants
  polished, evidence-backed writing about technical or complex subjects.When a user shares a
  brief or topic, interview them first using AskUserQuestion before drafting.
---

# Research Writing

Produce long-form prose that feels informed, carefully reasoned, and human. The goal is writing that earns trust through specificity, intellectual honesty, and restraint --- not through assertion or decoration.

These principles are distilled from close analysis of how skilled communicators write about complex, technical subjects for broad audiences. Internalize the reasoning behind each one so you can apply good judgment rather than follow rigid rules.

---

## Workflow: brief intake interview

When a user shares a brief, topic, or description of what they want written, don't jump straight into drafting. First, conduct a structured interview using the `AskUserQuestion` tool to surface the context, constraints, and details that separate good research writing from generic content. The brief alone rarely contains everything you need.

### Why this matters

Most writing briefs are underspecified. A user might say "write a blog post about our new API" but leave out the audience, the key differentiator, the evidence they have available, and what they want the reader to do after reading. The interview fills these gaps before you commit to a structure or voice, which saves significant rework later.

### How to conduct the interview

Read whatever the user has shared --- a brief, a doc, a rough outline, raw notes --- and then ask questions using `AskUserQuestion`. Don't ask obvious questions that the brief already answers. Instead, go deeper on what's missing or ambiguous.

**Round 1: Audience and intent.** Who is this for, and what should they take away? These two questions shape every structural and tonal decision that follows. A research report for investors reads differently than a blog post for developers, even if the underlying content is the same.

**Round 2: Evidence and specifics.** What concrete data, benchmarks, quotes, case studies, or examples does the user have available? Research writing lives or dies on specificity --- vague briefs produce vague prose. Push for numbers, names, and real outcomes. If the user doesn't have them yet, identify what they'd need to gather.

**Round 3: Structure and constraints.** What article type fits best (announcement, research report, narrative, industry piece)? Are there length targets, publication channels, or style guides to honor? Any topics to avoid or emphasize?

**Round 4: Edge cases and tradeoffs.** This is where the interview goes beyond the obvious. Ask about tensions in the material --- things like "you mention both speed and accuracy improvements, but are there cases where there's a tradeoff between them?" or "your brief focuses on the positive results, but are there limitations or caveats the audience should know about?" Surfacing these before drafting produces writing that feels honest rather than promotional.

Continue asking follow-up questions until you have enough context to draft confidently. Don't pad with unnecessary questions --- if the brief is already rich and specific, the interview can be short. The goal is to close the gaps, not to interrogate.

### After the interview

Synthesize what you've learned into a short internal outline before writing. This doesn't need to be shown to the user, but it should capture: the audience, the core message, the article type, the key evidence, and any constraints or caveats. Then proceed to drafting using the principles below.

---

## Core voice

The voice is confident but not boastful. Claims are backed by evidence; the writing lets results speak rather than asserting importance. The tone is warm and professional without being corporate or stiff. Think of a thoughtful colleague explaining something they know deeply and care about, not a press release or a sales pitch.

**First-person plural ("we") is natural when appropriate.** Use it when describing actions, decisions, or findings by a team or organization. Avoid it when it sounds presumptuous or when the subject isn't the author's group.

**Intellectual honesty is non-negotiable.** Acknowledge limitations, caveats, and uncertainty openly. Phrases like "this estimate comes with a high degree of uncertainty" or "the system certainly still lags behind the most skilled humans" build credibility rather than undermining it. Readers trust writers who tell them what they don't know.

**Be direct.** Say what you mean in the fewest words that preserve nuance. Avoid throat-clearing ("It is worth noting that..."), filler ("In order to..."), and hedging pileups ("It could potentially be argued that this might possibly..."). One well-placed hedge is honest; three stacked together is evasive.

---

## Structuring different article types

Different purposes call for different structures. Choose the one that fits your content, or blend elements as needed.

### Product and launch announcements

Open with a concise framing statement that tells the reader what matters and why. One or two sentences, not a paragraph of buildup. Then move through:

1. What's new --- capabilities and features, with specific details and numbers
2. Evidence --- benchmarks, evaluations, presented with precise figures and honest comparisons
3. Real-world validation --- partner quotes, early feedback, concrete use cases
4. Availability and practical details

Example opening rhythm:

> "The new release improves on its predecessor's coding skills. It plans more carefully, sustains agentic tasks for longer, and has better debugging skills to catch its own mistakes."

No "revolutionary" or "game-changing." Just what the thing does, stated plainly and specifically.

### Research reports

Frame with a clear research question. State what was studied, how, and why it matters, in the opening paragraphs. Organize findings into chapters or sections with descriptive (not clever) headers. Present quantitative results with appropriate precision and caveats. Use figures and data to anchor claims. Explain methodology accessibly but don't skip it.

Close by connecting findings to broader implications and acknowledging open questions. Research writing earns the right to speculate about the future by being rigorous about the present.

Example:

> "This report introduces new metrics of AI usage to provide a rich portrait of user interactions. These 'primitives' --- simple, foundational measures of how the product is used --- cover five dimensions relevant to economic impact."

The methodology is explained in plain language. Technical terms ("primitives") are introduced with a plain-English definition right next to them.

### Narrative and storytelling

Start with context that orients the reader, then go deep into specific cases. Use extended examples, individual researchers or organizations, and concrete details that make abstract concepts tangible.

Build from specific to general. A single lab's workflow, described in rich detail, teaches the reader more than a dozen abstract claims about "the future of science."

Example:

> "Consider a genome-wide association study --- a search for genetic variants linked to traits or diseases. Perfect pitch, for instance, has a strong genetic basis. Researchers take a large group of people and scan their genomes for variants appearing more frequently in one group than another."

A technical concept made vivid through a specific, relatable example (perfect pitch) --- not dumbed down but made accessible.

### Industry and vertical pieces

Frame around real problems that real people face. Open by establishing what the tools or capabilities enable in practical terms, then describe what's new, then show concrete use cases with enough detail that a reader in that industry can picture using them.

Partner quotes work best when they're specific about results, not generic praise. Prefer quotes that mention particular metrics, workflows, or outcomes.

---

## Sentence-level craft

### Specificity over assertion

Replace vague claims with concrete evidence. "Major improvement" means nothing; "a 10% lift in performance, reaching 68% vs. a 58% baseline" means something. Every number, comparison, or example you include makes the writing more credible.

**Example 1:**
Bad: "The system shows significant improvements across the board."
Good: "The new model scores 76% on the 8-needle retrieval benchmark, compared to 18.5% for the previous version."

### Explain technical terms in context

When introducing jargon, provide a natural parenthetical or appositive explanation. The reader should absorb the definition without feeling lectured.

Good: "The Gini coefficient, a standard measure of equality, fell from 0.37 to 0.32."
Bad: "The Gini coefficient fell. (Note: The Gini coefficient is a statistical measure of inequality.)"

### Vary sentence length and rhythm

Mix short declarative sentences with longer, more complex ones. A paragraph of uniformly long sentences is exhausting. A paragraph of uniformly short ones feels choppy and simplistic.

Short sentences work for emphasis, transitions, and landing key points. Longer sentences work for explanation, context, and connecting ideas. Let the content dictate the rhythm.

### Use em dashes purposefully

Em dashes are effective for inserting clarifications, asides, or pivots. Use them when parentheses would feel too tucked-away and commas would be ambiguous. Limit to one or two per paragraph at most --- overuse makes writing feel breathless and is a strong signal of AI-generated text.

### Active voice, mostly

Default to active voice. "We ran extensive safety evaluations" is clearer than "Extensive safety evaluations were run." But passive voice is fine when the actor is unknown, unimportant, or when you want to emphasize the object. Don't contort sentences to avoid it.

---

## Handling evidence and claims

**Benchmark data**: Present with specific numbers, name the benchmark, and include comparison points. Contextualize what the numbers mean for a reader who may not know the benchmark.

**Partner and customer quotes**: Choose quotes that are specific about outcomes, not generic endorsements. A quote like "The tool autonomously closed 13 issues and assigned 12 to the right team members in a single day" is vastly more useful than "We're excited about the partnership."

**Limitations and caveats**: State them plainly and in proximity to the claims they qualify. Don't bury caveats in footnotes or save them all for a disclaimer paragraph at the end. Weaving honesty throughout the piece builds more trust than a single disclaimer.

**Methodology**: Explain enough that a thoughtful reader understands how you arrived at your conclusions. The reader should never wonder "how do they know that?" without finding an answer nearby.

---

## Anti-content patterns: what to avoid

These patterns undermine credibility and signal promotional or AI-generated writing. They are drawn from common AI writing tells and should be treated as red flags during both drafting and review.

### Significance and hype inflation

Words like "revolutionary," "unprecedented," "game-changing," "groundbreaking," "pivotal," "testament," and "vital role" are almost never earned. If something is genuinely unprecedented, the evidence will make that clear without the adjective. Watch for "stands as," "serves as a reminder," "underscores the importance," "reflects broader trends," and "setting the stage for" --- these are filler that puffs up importance without adding information.

### Generic positive conclusions

"The future looks bright" and "exciting times lie ahead" say nothing. End with something specific: an open question, a concrete next step, or a finding that reframes how the reader thinks about the topic. Formulaic "Challenges and Future Prospects" sections are a dead giveaway of AI writing.

### Promotional and decorative language

Watch for "vibrant," "rich" (figurative), "profound," "nestled," "breathtaking," "stunning," "boasts a," "in the heart of," and "showcasing." These words inflate without informing. Replace them with specific, verifiable details.

### AI vocabulary words

These words appear far more frequently in AI-generated text than human writing: "Additionally," "delve," "foster," "garner," "interplay," "intricate/intricacies," "landscape" (abstract), "tapestry" (abstract), "underscore," and "showcase." They aren't banned, but if several appear together in the same passage, the writing will read as generated.

### Stacked hedging

One qualifier is honest. "This estimate comes with uncertainty" is good. "It could potentially be argued that this might possibly suggest" is cowardice dressed as precision.

### Synonym cycling (elegant variation)

Don't rotate through synonyms for the same concept to avoid repetition. If you're talking about "the model" throughout a paragraph, calling it "the system," "the tool," "the platform," and "the solution" in consecutive sentences is worse than just saying "the model" each time. Repetition of a precise term is clarity; artificial variation is noise.

### Structural tells

Avoid inline-header vertical lists (bolded term followed by colon on every bullet), the rule of three forced onto ideas that don't naturally group that way, negative parallelisms ("It's not just about X; it's about Y"), false ranges ("from X to Y, from A to B" where X and Y aren't on a meaningful scale), excessive boldface, and copula avoidance ("serves as" / "stands as" instead of plain "is").

### Sycophantic and servile tone

Never start with "Great question!" or "That's an excellent point." Avoid "I hope this helps!" and "Let me know if you'd like me to expand on any section." Just write the content.

### Filler phrases

Cut: "It is important to note that," "In order to," "It is worth mentioning that," "At the end of the day," "Due to the fact that," "At this point in time," "has the ability to." These add words without adding meaning.

---

## What ties it all together

The best writing in this style reads like it was written by someone who genuinely understands the subject, cares about getting it right, and respects the reader's intelligence. A few ways this manifests:

**Complexity is acknowledged, not hidden.** When results are mixed or uncertain, the writing says so. When a topic has genuine tension, both sides are addressed as a natural part of explaining the full picture --- not in a formulaic "on the other hand" way.

**The writing earns its conclusions.** Every claim in the final paragraphs should feel inevitable given what came before. If a claim isn't supported by the body of the piece, either add the evidence or cut the claim.

**Technical depth coexists with accessibility.** The writing doesn't talk down to experts or lose non-experts. It achieves this by being concrete: instead of simplifying a concept, it explains it through a specific example that makes the mechanism clear.

**Responsibility is woven in, not bolted on.** When relevant, discuss risks, limitations, and safeguards as a natural part of the narrative --- not as a separate section tacked onto the end.

**Forward-looking claims are grounded.** Anchor speculation in present evidence. "If sustained, usage per capita would be equalized across the country in 2-5 years" is grounded. "This will transform the industry" is not.

---

## Full workflow: interview, draft, humanize

The complete research-writing process has three phases. Each one addresses a different failure mode: the interview prevents writing from the wrong assumptions, the draft applies structural and tonal principles, and the humanizer pass catches residual AI patterns.

### Phase 1: Interview

When the user provides a brief or topic, conduct the brief intake interview described above using `AskUserQuestion`. Surface audience, evidence, structure, and tradeoffs. Skip this phase only if the user has already provided exhaustive detail or explicitly asks you to skip it.

### Phase 2: Draft

Write the full draft following the core voice, article structure, sentence craft, and evidence-handling principles in this skill. Use the interview context to make every choice --- from article type to tone to which caveats to surface --- grounded in what you learned.

### Phase 3: Humanizer pass

After the draft is complete, invoke the `humanizer` skill as a second pass. The humanizer scans for the full catalog of AI writing tells (24 pattern categories) and rewrites problematic sections. It is specifically designed to catch patterns that are easy to miss during drafting: em dash overuse, synonym cycling, promotional language, significance inflation, rule-of-three forcing, sycophantic tone, and structural tells like inline-header bullet lists.

After the humanizer runs, review its output to make sure it preserved the intended meaning, tone, and technical accuracy. The humanizer optimizes for naturalness, which occasionally conflicts with precision --- if it simplified a technical claim too aggressively or flattened a nuance that matters, restore the original.

Final check: read the piece aloud (mentally). Does it sound like a person talking, or a machine assembling plausible sentences? If any sentence makes you pause, revise it.