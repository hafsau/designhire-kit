# Portfolio Pitch

Tailor your portfolio presentation for a specific company and role.

## Usage

```
/portfolio-pitch
```

Then provide the company name, role, and job description.

## What It Does

1. Analyzes the company and role requirements
2. Recommends which case studies to present (ordered by business impact)
3. Tells you what to emphasize vs skip
4. Provides a narrative thread connecting your work to their needs
5. Suggests how to frame each project for this specific audience
6. **Ensures your case studies lead with outcomes, not process**

## Core Principle: Business Impact First

Modern hiring managers (2025+) filter portfolios in 30 seconds. They're looking for:
- **Business outcomes** — revenue, conversion, efficiency metrics
- **Decision-making ability** — why you chose what you chose
- **Shipped work** — not just concepts or explorations

Pretty visuals won't save a weak case study. Impact will.

## Instructions for Claude

When the user runs `/portfolio-pitch`:

1. Read context files:
   - `context/resume.md` for background
   - `context/portfolio.md` for case studies
   - `context/writing-style.md` for tone

2. **Check if context files are filled in.** If they contain placeholder text, ask the user to provide: their case studies with brief descriptions.

3. Ask for:
   - Company name
   - Role title
   - Job description (paste it)
   - Presentation format (live walkthrough, recorded video, PDF deck, or portfolio website review)
   - Time limit (if any)

4. Analyze the job description for:
   - Key skills they're looking for
   - Design challenges they face
   - Company stage and culture signals
   - Specific technologies or methods mentioned

5. Generate a portfolio pitch guide:

### Case Study Selection

Recommend 2-3 case studies based on relevance:

```
For this [Role] at [Company]:

LEAD WITH: [Case Study Name]
- Why: [Connection to their needs]
- Emphasize: [Specific aspects]
- Time: [X minutes]

SECOND: [Case Study Name]
- Why: [Connection to their needs]
- Emphasize: [Specific aspects]
- Time: [X minutes]

OPTIONAL THIRD: [Case Study Name]
- Only if: [Condition — they ask, time permits, etc.]

SKIP: [Case Study Name]
- Why: [Not relevant to this role]
```

### Narrative Thread

Provide a connecting story:

```
Your through-line for this presentation:

"I solve [type of problem] by [your approach].
At [Company 1], this meant [specific example].
At [Company 2], I applied the same thinking to [different context].
For [Target Company], I'd bring this to [their specific challenge]."
```

### Per-Project Talking Points

For each recommended case study:

```
[Case Study Name]

Opening hook (1 sentence):
"[Specific, attention-grabbing summary]"

Key points to hit:
1. [Point] — connects to [their requirement]
2. [Point] — connects to [their requirement]
3. [Point] — connects to [their requirement]

Metric to emphasize:
"[Specific number and what it means]"

Transition to next project:
"[How this connects to the next case study or their needs]"
```

### What to Skip or Minimize

```
DON'T spend time on:
- [Aspect] — not relevant to this role
- [Aspect] — they likely don't care about this

DON'T mention:
- [Thing that might raise concerns]
- [Thing that's not impressive for this level]

If they ask about [topic you're weak on]:
"[How to redirect or address honestly]"
```

### Questions to Prepare For

Based on what you're presenting:

```
They'll likely ask:
- "[Question based on your case study]"
  Your answer: [Brief talking point]

- "[Question about their specific challenge]"
  Your answer: [How to connect to your experience]

- "[Question about gap in your experience]"
  Your answer: [Honest pivot]
```

### Case Study Structure Template

For each case study, ensure it follows this structure:

```
1. OUTCOME FIRST (10% of time)
   "This project increased [metric] by [X%]"
   Start with the result, not the problem

2. CONTEXT (10%)
   Company, timeline, your role, team size
   Keep this brief — they'll ask if they want more

3. PROBLEM (15%)
   What was broken? Why did it matter?
   Use metrics: "40% error rate" not "users struggled"

4. PROCESS (50%)
   This is where you show HOW you think:
   - Research methods and key insights
   - Design decisions and tradeoffs
   - Iteration based on feedback
   - Collaboration with eng/PM

   Show your work. Hiring managers want to see your process.

5. RESULT (15%)
   Specific metrics, user feedback, business impact
   Connect back to the opening outcome
```

### 2025+ Expectations

Modern design hiring has shifted. Address these in your pitch:

**AI Tools Usage:**
- If you use Figma AI, ChatGPT, or other AI tools — mention it
- Framing: "I use AI for [X] which lets me focus on [Y]"
- Don't hide it; embracing tools shows you're current

**Niche vs Generalist:**
- Senior roles increasingly want specialists
- Position yourself: "I specialize in [X] but can do [Y]"
- Example: "I focus on complex B2B tools, but I've done consumer work"

**Shipped Work Only:**
- Concepts and explorations are secondary
- Lead with work that's live and measurable
- If you only have concept work, frame why (NDA, startup failed, etc.)

6. Output the complete pitch guide.

### Phase 7: Hiring Manager Review (Built-In Evaluation)

7. **Put on your design hiring manager hat** and evaluate the pitch:
   - Would this portfolio pitch make you want to hire this person?
   - Are the case studies clearly connected to the role's needs?
   - Is the narrative compelling or generic?
   - What's missing that would make the pitch stronger?

Include this evaluation in the output:

```
## Hiring Manager Review

**Putting on my design hiring manager hat:**

**Would I move forward with this candidate?** [YES / MAYBE / NO]

**What's compelling:**
- [Specific strengths of the pitch for THIS role]

**What's weak or missing:**
- [Gaps, unconvincing parts, or concerns]

**To make this pitch stronger:**
- [Specific, actionable recommendations]
```

### 30-Second Filter Test

Before presenting your recommendations, check:

```
For each case study, can a hiring manager understand in 30 seconds:
- [ ] What the project achieved (metric/outcome)
- [ ] What you specifically did (not the team)
- [ ] Why it matters to THEIR company

If NO to any → restructure the pitch to front-load these
```

## Example Output

```
# Portfolio Pitch: Senior Product Designer at Linear

## Case Study Selection

LEAD WITH: Stackflow Analytics Dashboard
- Why: They're building productivity tools; you redesigned a complex dashboard for clarity
- Emphasize: Information hierarchy decisions, how you reduced time-to-insight
- Time: 12-15 minutes
- Connect to: Linear's focus on speed and keyboard-first design

SECOND: Medley Design System
- Why: Job mentions "systems thinking" and they have a mature design system
- Emphasize: Token architecture, cross-platform consistency, governance
- Time: 8-10 minutes
- Connect to: Scaling design across their product suite

SKIP: MedTrack Healthcare App
- Why: Healthcare domain not relevant; save for questions if they ask about accessibility

## Narrative Thread

"I make complex tools feel simple. At Stackflow, that meant turning a data-heavy dashboard into something you could glance at and understand. At Medley, it meant building a design system that 15 engineers could use without hand-holding. For Linear, I'd bring that same focus on removing friction — especially for power users who live in your product all day."

## Stackflow Talking Points

Opening hook:
"Users were churning because they couldn't find insights in our analytics dashboard. I fixed that by showing less, not more."

Key points:
1. Progressive disclosure approach — connects to Linear's minimal UI philosophy
2. Removed 40% of visible metrics — connects to their "opinionated product" culture
3. Designed for keyboard users first — directly relevant to Linear's interaction model

Metric to emphasize:
"Time-to-insight dropped from 3 minutes to 30 seconds"

Transition:
"That project taught me how to make decisions for users, not just give them options. I applied the same philosophy when building Medley's design system..."

## Questions to Prepare For

They'll likely ask:
- "How did you decide what to remove from the dashboard?"
  Answer: User session analysis + talking to churned users. Data showed which metrics nobody clicked.

- "How do you handle disagreement with PMs or eng?"
  Answer: Reference the design system governance story — sometimes you compromise, sometimes you stand firm.

- "You haven't worked on developer tools before."
  Answer: "True, but power users are power users. The Stackflow dashboard was used by analysts who lived in it 8 hours a day — same intensity as Linear users."
```

## Notes

- Always connect case studies to THEIR problems, not just your accomplishments
- Recommend a time allocation that leaves room for questions
- Include what to skip — this is as important as what to show
- Prepare redirects for weak areas
- Adjust formality based on company culture (startup vs enterprise)
- **Lead with business impact** — metrics in the first 30 seconds
- **Show process** — 50% of presentation should be how you think
- **Be specific about your role** — "I led" vs "the team did"
- Address AI tool usage proactively if relevant to the role
