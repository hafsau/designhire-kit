# LinkedIn Outreach Message

Generate a short, personal LinkedIn message to a hiring manager or recruiter that doesn't sound like every other applicant.

## Usage

```
/linkedin-outreach
```

Then provide:
1. The person's name and role (e.g., "Sarah Chen, Design Lead at Figma")
2. The job you applied for
3. (Optional) Something specific about them or the company's design work

## What It Does

1. Reads your context files for relevant background
2. Generates a 3-5 sentence LinkedIn message that:
   - Feels personal, not templated
   - References something specific about them or the company
   - Mentions you applied and one strong reason you're a fit
   - Has a soft ask, not a hard sell
   - Sounds like a real person, not an AI

## Instructions for Claude

When the user runs `/linkedin-outreach`:

1. Read context files:
   - `context/resume.md` for background
   - `context/portfolio.md` for case studies
   - `context/writing-style.md` for tone

2. **Check if context files are filled in.** If they contain placeholder text, ask the user to provide: name, current role, 1-2 relevant projects, preferred tone.

3. Ask for:
   - Who they're messaging (name, role, company)
   - The role they applied for
   - Anything specific they know about this person or the company's recent design work

4. Generate a LinkedIn message following these rules:

**Structure:**
- Opening: Friendly greeting + specific reference to their work or the company (NOT "I hope this message finds you well")
- Middle: Mention you applied + one concrete reason you're a good fit
- Closing: Soft ask or conversation starter (NOT "I'd love to pick your brain")

**Tone Rules:**
- Casual but professional
- NO "I hope this finds you well"
- NO "I'd love to connect" (everyone says this)
- NO "pick your brain" (cringe)
- NO multiple exclamation points
- Reference something real about them or the company
- Sound like you'd be fun to work with

**Length:** 3-5 sentences max. LinkedIn messages should be skimmable.

5. Output the message ready to copy.

## Example Outputs

**Good Example 1 (referencing their work):**
```
Hi Sarah — I just applied for the Design Engineer role at Figma. I noticed you led the new variable fonts feature. The way you handled the complexity of the preview panel is similar to a challenge I tackled in my healthcare app (progressive disclosure for medication options). Would love to hear how your team approached the technical constraints.
```

**Good Example 2 (referencing company):**
```
Hey Marcus — I applied for the Product Designer role today. I've been following Linear's design system work and the way you've handled keyboard navigation is impressive. I built something similar for an accessibility-first healthcare product. Happy to share what I learned if useful.
```

**Good Example 3 (recruiter):**
```
Hi Jamie — I just applied for the Senior Designer role at Stripe. My background is in complex B2B tools (fintech and healthcare), and I've shipped design systems at scale. The Dashboard work Stripe's team has done is exactly what I want to be building. Would love to chat if the fit looks good.
```

### Example 4: No Specific Info About Person
```
Hi [Name] — I applied for the Product Designer role at [Company] today. I've been following your design blog — the recent post about your icon system redesign was exactly the kind of systems problem I love solving. Built something similar at my last company. Would be great to chat if the role's still open.
```

### Example 5: Cold Outreach (No Open Role)
```
Hi [Name] — I've been using [Product] daily for the past year and the recent [Feature] update is impressive. I'm a product designer focused on complex tools, and I'd love to be part of what you're building. Not sure if you're hiring, but wanted to reach out. Happy to share my portfolio if useful.
```

**Bad Examples (don't do this):**
```
❌ "I hope this message finds you well! I'm reaching out because I'm very interested in the role..."

❌ "Hi! I'd love to connect and learn more about opportunities at your amazing company!"

❌ "Dear Hiring Manager, I am writing to inquire about the position..."
```

## Notes

- If you know something specific about the person, use it
- If not, reference the company's recent design work
- Always connect to your own relevant experience
- End with a soft conversation starter, not a demand
- Keep it SHORT — recruiters get hundreds of these
