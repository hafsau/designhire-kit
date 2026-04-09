# Cover Letter Generator

Generate a portfolio-aware cover letter that sounds human and references your actual work.

## Usage

```
/cover-letter
```

Then paste the job description when prompted.

## What It Does

1. Reads your resume from `context/resume.md`
2. Reads your portfolio case studies from `context/portfolio.md`
3. Reads your writing style preferences from `context/writing-style.md`
4. **Researches the company** before writing
5. Analyzes the job description you provide
6. Generates a 3-4 paragraph cover letter that:
   - Opens with something specific about why this role interests you
   - Connects your portfolio work to their needs
   - References specific metrics from your experience
   - Sounds like a confident designer, not a generic applicant
   - Ends with a clear call to action (not "I look forward to hearing from you")

## Instructions for Claude

When the user runs `/cover-letter`:

### Phase 1: Context Gathering

1. First, read the user's context files:
   - `context/resume.md` for their background
   - `context/portfolio.md` for case studies and metrics
   - `context/writing-style.md` for tone preferences

2. **Check if context files are filled in.** If they contain placeholder text like "[Your Name]" or template instructions, ask the user to either:
   - Fill in the context files first, OR
   - Provide quick info now: name, current role, 1-2 relevant projects with metrics, preferred tone

3. Ask the user to paste the job description.

### Phase 2: Company Research (Before Writing)

4. **Research the company before drafting.** Use web search to find:
   - Recent product launches or design updates
   - Blog posts about their design process
   - Team structure (who's on the design team)
   - Recent news, funding, or company changes
   - Their design system (if public)

   This research should inform specific references in the letter. Don't just write generic praise.

5. Analyze the job description for:
   - Company name and what they do
   - Key responsibilities and requirements
   - Design challenges they face
   - Skills they're looking for
   - **Tone signals** — is this a startup (casual) or enterprise (formal)?

### Phase 3: Matching & Tone Calibration

6. Match the user's experience to the job:
   - Which case studies are most relevant?
   - What metrics demonstrate relevant skills?
   - What unique angle can they bring?

7. **Calibrate tone to match the company:**
   - Startup (<50 people): Casual, direct, personality-forward
   - Growth stage (50-500): Professional but warm
   - Enterprise (500+): More formal, emphasize scale and process
   - Read their job posting language and mirror it

### Phase 4: Writing

8. Generate a cover letter following these rules:

**Structure:**
- Opening (1 paragraph): Why this specific role/company excites you. Be specific — mention their product, recent work, or mission. Don't be generic.
- Middle (1-2 paragraphs): Connect your portfolio work to their needs. Reference specific case studies by name. Use metrics.
- Closing (1 paragraph): Clear call to action. Not "I look forward to hearing from you" — something specific like "I'd love to walk you through how I approached the MedRec redesign" or "Let's chat about how I could help [specific challenge]."

**Tone Rules (from CLAUDE.md humanizer):**
- No "I am writing to express my interest"
- No "esteemed organization" or similar inflated language
- No em-dash overuse
- No "leverage," "synergy," "robust," or other AI-giveaway words
- Use first person naturally
- Vary sentence length
- Have opinions and personality

**Length:** 250-400 words. Hiring managers skim — be concise.

7. Output the cover letter in a clean format, ready to copy.

## Example Outputs

### Example 1: B2B SaaS Role (Senior Level)
```
Hi [Hiring Manager],

I saw the Product Designer role at Acme and got excited — you're building exactly the kind of complex B2B tool I love working on. The way you've approached data visualization in your recent dashboard update reminded me of the challenges I tackled at [Company].

My most relevant work is MedRec, a diabetes management app I designed for Kaiser. The existing interface had a 40% error rate in medication logging because users were overwhelmed by options. I redesigned the core workflow using progressive disclosure and reduced errors by 35%. That experience with healthcare compliance and error-reduction feels directly applicable to [specific thing from their JD].

I also built [Portfolio Company]'s design system from scratch, going from inconsistent components to a unified library that cut design-to-dev time by 50%. I know you're scaling your design team, and I've been through that process.

I'd love to walk you through my MedRec case study and discuss how I could help [specific challenge]. What does your calendar look like next week?

Best,
[Name]
```

### Example 2: Startup Role (Scrappy Tone)
```
Hey team,

Your job post mentioned you're looking for someone comfortable with ambiguity. That's my comfort zone.

At my last startup, I was the only designer for 8 months. I shipped a complete onboarding redesign in 3 weeks that improved activation by 18% — no design system, no researchers, just me and a lot of user calls. I've since learned the value of process, but I still know how to move fast when it matters.

I saw you're rebuilding the dashboard. I did something similar at Stackflow — took a "powerful but confusing" analytics tool and made it actually usable. Time-to-insight dropped from 3 minutes to 30 seconds. Happy to share how.

What's the best way to continue the conversation?

[Name]
```

### Example 3: Enterprise Role (Formal Tone)
```
Dear Hiring Manager,

I'm writing regarding the Senior Product Designer position on the Enterprise Platform team.

My background is in designing complex B2B applications for regulated industries. At Medley Health, I led the redesign of a medication management system used by 50,000+ patients. The project required balancing strict compliance requirements with usability — we reduced error rates by 76% while maintaining HIPAA compliance.

I've also built and maintained design systems at scale. My component library at Medley serves 3 products and 15 engineers, with documented accessibility standards that brought our audit pass rate from 60% to 94%.

I'd welcome the opportunity to discuss how my experience with enterprise-scale design challenges could contribute to your platform team.

Best regards,
[Name]
```

## Quality Checks (Before Output)

Before presenting the final letter, run these internal checks:

### Specificity Test
Ask yourself: "Could this letter be sent to a different company by changing the name?"
- If YES → rewrite with more specific references
- If NO → good to go

The letter should reference:
- Something specific about THEIR product, design, or recent work
- A specific challenge from THEIR job description
- Why YOUR experience connects to THEIR situation

### Quantification Check
The letter MUST include at least one metric:
- Revenue/conversion impact: "increased signups by 23%"
- Efficiency gains: "reduced time-to-task by 40%"
- Scale: "design system used by 15 engineers across 3 products"
- Error reduction: "decreased support tickets by 30%"

If the user's portfolio lacks metrics, ask them for approximate numbers before writing.

### Audience Audit
Before finalizing, check:
- [ ] Does the opening hook grab attention in the first sentence?
- [ ] Is the company research visible (not generic praise)?
- [ ] Does the tone match the company culture?
- [ ] Are case studies referenced by name with metrics?
- [ ] Is the CTA specific, not generic?
- [ ] Would a hiring manager read past the first paragraph?

### Recruiter Review (Built-In Evaluation)

After generating the cover letter, **put on your senior recruiter hat** and evaluate it:

Include this in the output:

```
## Recruiter Review

**Putting on my senior recruiter hat (reviewed 10,000+ applications):**

**First Impression:**
[Would I keep reading after the first paragraph? Why/why not?]

**What works:**
- [Specific strengths of this letter]

**What's weak:**
- [What might make me skeptical or lose interest]

**Verdict:** [STRONG / GOOD / NEEDS WORK / WEAK]

**To improve before sending:**
- [Specific, actionable suggestion]
```

This evaluation should be honest — a lukewarm letter that gets sent is worse than a strong letter that took another revision.

## Notes

- Always reference at least one case study by name
- Always include at least one metric
- Match the formality level to the company (startup vs enterprise)
- If they mention specific technologies or methods, connect to your experience with them
- Do company research BEFORE writing — this is what makes it specific

## When Experience Doesn't Match Directly

If the user's portfolio doesn't directly match the job requirements:

1. **Find transferable skills** — Complex healthcare UI → Complex fintech UI. Design system work → Any systems thinking role.

2. **Acknowledge the gap honestly** — Don't pretend. Say something like: "I haven't worked in [industry] specifically, but my work on [project] involved similar challenges: [specific parallel]."

3. **Lead with learning ability** — Reference a time you ramped up quickly on something unfamiliar.

4. **Focus on problem-solving patterns** — "I haven't designed for developers, but I've designed for power users who need efficiency over hand-holding — same principle."

**Example for career switcher:**
```
I'm coming from [previous field], which might seem unrelated, but the core challenge is the same: [specific parallel]. At [Company], I [specific example that shows transferable skill]. I'd bring that same approach to [their challenge].
```

**Example for industry switch:**
```
Most of my work has been in healthcare, not fintech. But both require designing for high-stakes decisions where errors have real consequences. My MedRec project dealt with similar constraints: compliance requirements, complex data, users who need speed and accuracy.
```
