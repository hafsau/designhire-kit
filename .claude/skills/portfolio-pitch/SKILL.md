# Portfolio Pitch

Tailor your portfolio presentation for a specific company and role.

## Usage

```
/portfolio-pitch
```

Then provide the company name, role, and job description.

## What It Does

1. Analyzes the company and role requirements
2. Recommends which case studies to present
3. Tells you what to emphasize vs skip
4. Provides a narrative thread connecting your work to their needs
5. Suggests how to frame each project for this specific audience

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

6. Output the complete pitch guide.

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
