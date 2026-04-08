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
2. Generates a **300-500 character** LinkedIn message that:
   - Feels personal, not templated
   - References something specific about them or the company
   - Mentions you applied and one strong reason you're a fit
   - Has a soft ask, not a hard sell
   - Sounds like a real person, not an AI

## Key Stats (2025 Data)

- Messages under 500 characters get **22% better response rates**
- Personalized messages get **27% more responses** than templates
- Connection requests with notes: **58% higher acceptance**
- Best send times: **Tuesday-Thursday, 10 AM-2 PM**
- LinkedIn messages outperform InMails 2-3x (25-35% vs 10-15% response)

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

**Length:** 300-500 characters (3-5 sentences). LinkedIn messages should be skimmable.

**Personalization Formula (CCQ Method):**
- **Compliment**: Reference specific work they've done (not generic praise)
- **Commonality**: Shared experience, interest, or connection
- **Question**: Soft engagement hook that invites response

**90/10 Rule:** Message should mention them/their work 90%, yourself 10%

5. Output the message ready to copy, with character count.

### Message Type Strategy

**For connection requests (300 char limit):**
- Shorter, focused on one specific detail
- Don't pitch — just establish relevance
- Save the full context for after they accept

**For direct messages to 1st-degree connections:**
- Can go up to 500 characters
- Include your reason for reaching out
- Reference specific work + your relevant experience

**For InMail (use sparingly — lower response rates):**
- Only use when other methods fail
- Craft compelling subject line
- Worth the cost only for senior/hard-to-reach contacts

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

## Timing & Follow-Up

**Best times to send:**
- Tuesday-Thursday, 10 AM-2 PM (highest engagement)
- Avoid Monday mornings and Friday afternoons

**Follow-up cadence (if no response):**
- Day 1: Initial message
- Day 5-6: First follow-up (different angle, add value)
- Day 12: Final follow-up (shorter, acknowledge busy)
- After Day 14: Move on — don't follow up again

**Never:**
- Send the same message twice
- Follow up more than 2 times
- Send on weekends

## Notes

- If you know something specific about the person, use it
- If not, reference the company's recent design work
- Always connect to your own relevant experience
- End with a soft conversation starter, not a demand
- Keep it SHORT — recruiters get hundreds of these
- **Count characters** — stay under 500 for best results
- **Research their activity** — recent posts, promotions, articles give you hooks
