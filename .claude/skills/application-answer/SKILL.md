# Application Answer Generator

Generate thoughtful, specific answers to common job application questions.

## Usage

```
/application-answer
```

Then paste the question(s) you need to answer.

## What It Does

1. Reads your context files for relevant background
2. Analyzes the question to understand what they're really asking
3. Generates a specific, portfolio-backed answer that:
   - Actually answers the question (not generic fluff)
   - References real projects and metrics
   - Shows personality and thinking process
   - Fits the typical word limit (150-300 words unless specified)

## Instructions for Claude

When the user runs `/application-answer`:

1. Read context files:
   - `context/resume.md` for background
   - `context/portfolio.md` for case studies
   - `context/writing-style.md` for tone

2. **Check if context files are filled in.** If they contain placeholder text, ask the user to provide: name, relevant experience, 1-2 projects with metrics.

3. Ask user to paste the application question(s).

4. For each question, identify:
   - What they're REALLY asking (underlying intent)
   - Which experience from the portfolio is most relevant
   - What metric or outcome demonstrates this skill

5. Generate an answer following these rules:

**Structure:**
- Lead with the answer, not the backstory
- Support with a specific example
- Include a metric or outcome when possible
- End with what you learned or how you'd apply it

**Tone Rules:**
- Direct and specific, not vague
- First person, conversational
- Show your thinking process
- Don't oversell or use superlatives
- Avoid AI-giveaway phrases

**Length:**
- Short questions: 100-200 words
- "Tell us about..." questions: 200-300 words
- Follow any word limits specified

6. Output answers clearly labeled by question.

## Common Question Types

### "Tell us about a time you..."
Answer with the STAR method (Situation, Task, Action, Result) but lead with the result:
```
I reduced medication logging errors by 35% at Kaiser by redesigning their diabetes management workflow.

The original interface presented 40+ options on one screen, overwhelming users during time-sensitive moments. I ran usability tests, identified the key friction points, and implemented progressive disclosure — showing only the 5 most common options first, with expansion for edge cases.

The result: error rates dropped from 40% to 5%, and user satisfaction scores went from 2.1 to 4.2 (out of 5).
```

### "Why do you want to work here?"
Be specific about the company, not generic:
```
I want to work at Linear because you're solving a problem I care deeply about — making tools that respect users' time. I've been using Linear for two years and the keyboard-first approach influenced how I designed the accessibility features in my healthcare app.

Your recent work on the mobile app shows you're not just copying desktop patterns — you're rethinking what project management should feel like on different form factors. That's the kind of design thinking I want to be part of.
```

### "What's your design process?"
Don't recite a textbook process — show how you adapt:
```
My process depends on the constraints. For a recent 2-week sprint at [Company], I skipped formal research and used sales call recordings to understand user pain points — we didn't have time for interviews, but we had hundreds of hours of real conversations.

For longer projects like MedRec (6 months), I ran longitudinal studies and diary entries because the problem required understanding behavior over time, not just in-the-moment reactions.

The constant: I start with the problem, not the solution. I've scrapped designs 3 weeks in because user testing showed we were solving the wrong thing.
```

### "What's a challenge you faced and how did you overcome it?"
Pick a real challenge, not a humble-brag:
```
At [Company], I pushed hard for a redesign that the engineering team resisted — they were worried about migration complexity. I was frustrated, but I was also wrong about how I approached it.

Instead of presenting a final design and asking them to build it, I should have involved them earlier. I changed my approach: we did a design spike together where they helped me understand the technical constraints, and I helped them see the UX wins.

The final design was 60% of my original vision, but it shipped in half the time and the engineers owned it. Now I co-design with engineering from day one.
```

## Notes

- Always use real examples from your portfolio
- Include metrics when you have them
- If you don't have a perfect example, be honest about adaptation
- Show self-awareness and growth
- Don't answer questions you weren't asked

## When You Don't Have Direct Experience

If the question asks about something not in the user's portfolio:

1. **Find the closest parallel** — "I haven't led a design system from scratch, but I contributed to one and understand the challenges..."

2. **Be honest, then pivot** — "I don't have direct experience with [X], but I faced a similar challenge when [related example]."

3. **Show learning ability** — Reference how quickly you've ramped up on unfamiliar things before.

4. **Don't make things up** — Never invent experience. It's better to show self-awareness than to lie.

**Example answer for missing experience:**
```
I haven't managed designers directly, but I've led cross-functional projects where I was responsible for coordinating work across 3 engineers and a PM. The core skills are the same: clear communication, removing blockers, and creating space for people to do their best work. I'd bring that same approach to managing a design team.
```

**Example for "tell me about a failure":**
```
At [Company], I spent 3 weeks on a redesign before testing it — and users hated it. I'd assumed the problem was visual hierarchy, but the real issue was information architecture. I should have tested earlier. Now I run quick validation within the first week of any project, even if it's just 3 users and a paper prototype.
```
