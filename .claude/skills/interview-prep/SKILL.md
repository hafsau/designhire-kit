# Interview Prep

Generate likely interview questions, talking points, and portfolio presentation guidance for a specific role.

## Usage

```
/interview-prep
```

Then provide the company name, role, and job description.

## What It Does

1. Analyzes the job description and company
2. Generates likely interview questions based on the role
3. Creates talking points that connect your portfolio to their needs
4. Provides portfolio presentation guidance
5. Suggests questions to ask them
6. **Prepares you for modern interview formats** (whiteboard, AI exercises, etc.)

## 2025 Interview Landscape

- **60% of interview questions are behavioral** — prepare STAR stories
- **AI literacy is expected** — be ready to discuss how you use AI tools
- **Portfolio presentations are two-way** — seek feedback, don't just present
- **Whiteboard challenges test process** — aesthetics matter less than thinking

## Instructions for Claude

When the user runs `/interview-prep`:

1. Read context files:
   - `context/resume.md` for background
   - `context/portfolio.md` for case studies
   - `context/writing-style.md` for tone and personality

2. **Check if context files are filled in.** If they contain placeholder text, ask the user to provide: name, current role, 2-3 key projects with metrics, and any specific strengths to emphasize.

3. Ask for:
   - Company name
   - Role title
   - Job description (paste it)
   - Interview stage (phone screen, portfolio review, onsite, etc.)

4. Generate a comprehensive prep guide:

### Likely Questions

**Based on job description:**
- Parse requirements and generate questions that test each
- Example: If JD mentions "design systems," generate: "Tell me about a design system you've built. What were the key decisions?"

**Common design interview questions:**
- "Walk me through your process for [type of work they do]"
- "Tell me about a project that failed or was challenging"
- "How do you handle feedback you disagree with?"
- "How do you prioritize when everything is urgent?"
- "What's your approach to working with engineers?"

**Company-specific:**
- Based on their values, culture, recent work
- Example for Figma: "How do you think about designing for designers?"

### Talking Points

For each major point in the job description, provide:
- The requirement they listed
- Which of your projects demonstrates this
- The specific story/metric to reference
- How to frame it

Example:
```
Requirement: "Experience with complex data visualization"

Your project: MedRec diabetes management app

Talking point: "At MedRec, I designed a glucose tracking interface that needed to show 90 days of data while remaining actionable. The key insight was showing trends, not individual points — users needed to see patterns, not numbers. I can show you how I iterated on this."

Metric to mention: "Reduced time-to-insight from 3 minutes to 30 seconds"
```

### Portfolio Presentation Guidance

Based on the role, recommend:
- Which 2-3 case studies to lead with
- What aspects to emphasize
- What to skip or minimize
- How long to spend on each
- How to connect projects to their problems

Example:
```
For this Design Engineer role at Figma:

Lead with: MedRec (shows technical design skills)
- Emphasize: Accessibility implementation, design-to-code process
- Spend: 10-15 minutes
- Connect to: Their focus on "design for designers" — show you can build complex UIs

Second: Design System work
- Emphasize: Token architecture, cross-platform considerations
- Spend: 8-10 minutes
- Connect to: Figma's own design system evolution

Skip: Brand work from early career (not relevant)
```

### Questions to Ask Them

Generate thoughtful questions that show you've done research:
- About the team structure and collaboration
- About their current design challenges
- About the role's impact
- About growth and learning

Avoid generic questions like "What's the culture like?"

Example good questions:
- "I noticed you recently shipped [feature]. How does the design team handle post-launch iteration?"
- "What's the biggest design challenge you're facing that this role would help with?"
- "How do designers here influence the product roadmap?"

5. Output a structured prep document.

### Whiteboard Challenge Framework

If the interview includes a design challenge, prepare:

**5-Step Process (30-60 min typical):**
1. **Ask Questions (5 min)** — Never start designing immediately. Ask about users, constraints, success metrics
2. **Focus on Users (5 min)** — Map the user story/journey before any UI
3. **Outline Flow (10 min)** — Sketch key screens/states at high level
4. **Explore Alternatives (15-20 min)** — Generate 2-3 different approaches
5. **Converge + Summary (5 min)** — Pick one, explain tradeoffs, invite feedback

**Critical behaviors:**
- Talk through every choice aloud — silence is interpreted negatively
- Invite role-play: "Be a stakeholder while I..."
- Iterate on feedback openly — don't defend ideas defensively
- Acknowledge unknowns: "I don't know X, let me assume..."

### AI Fluency (2025 Expectation)

Be prepared to discuss:
- How you use AI tools (Figma AI, ChatGPT, Adobe Firefly) in your workflow
- Frame it as: "I use AI for [X] which lets me focus on [Y]"
- Show you're a curator/editor of AI output, not just a user
- If asked directly, don't hide it — embracing tools shows you're current

### Common Mistakes to Avoid

**Portfolio presentation:**
- Starting with solutions instead of problem context
- Using only "we" language without owning individual contributions
- Presenting without a cohesive narrative/POV
- Vague impact descriptions ("improved the UX")

**Behavioral questions:**
- Not using STAR structure (60% of time should be on Action)
- Deflecting credit entirely to team
- Criticizing former employers or colleagues

**Design challenges:**
- Starting to sketch before asking questions
- Not seeking clarification on constraints
- Defending ideas instead of iterating on feedback
- Going silent while thinking (narrate your process)

### What Gets Offers (vs Rejections)

Top candidates demonstrate:
1. **Structured problem-solving narrative** — not just pretty designs
2. **Clear ownership language** — "I decided to..." not "we ended up..."
3. **Business impact quantification** — even estimated metrics beat none
4. **Graceful handling of feedback** — iteration mindset, not defensiveness
5. **Thoughtful questions that show research** — not generic "what's the culture like?"

## Notes

- Tailor everything to the specific role and company
- Prioritize depth over breadth — they can't ask everything
- Include both behavioral and portfolio questions
- Help them prepare for awkward questions (gaps, failures, etc.)
- **Mock interview practice is non-negotiable** — record yourself, critique, iterate
