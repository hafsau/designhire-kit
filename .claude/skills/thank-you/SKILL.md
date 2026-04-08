# Thank You Email

Generate a thoughtful post-interview thank you email that stands out from generic templates.

## Usage

```
/thank-you
```

Then provide:
1. Who you interviewed with (name, role)
2. What you discussed
3. Anything specific that came up

## What It Does

1. Generates a personalized thank you email that:
   - References something specific from the conversation
   - Reinforces why you're a good fit
   - Addresses any concerns that came up
   - Feels genuine, not templated

## Instructions for Claude

When the user runs `/thank-you`:

1. Read context files:
   - `context/resume.md` for the user's name
   - `context/writing-style.md` for tone preferences

2. **Check if context files are filled in.** If name is a placeholder, ask the user for their name.

3. Ask for:
   - Interviewer's name and role
   - What you discussed (topics, projects, questions)
   - Anything specific that resonated or that you want to follow up on
   - Any concerns or hesitations that came up
   - Timeline mentioned (if any)

4. Generate a thank you email following these rules:

**Structure:**
- Opening: Thank them + reference something specific from the conversation
- Middle: Reinforce fit based on what you discussed
- Optional: Address any concerns or provide additional info
- Closing: Express continued interest + acknowledge their timeline

**Tone Rules:**
- Warm but professional
- NOT "Thank you for your time" (generic)
- NOT "I really enjoyed our conversation" (empty)
- Reference a real moment from the interview
- Short — 4-6 sentences max

**Timing:**
- Send within 24 hours
- Same day is ideal
- Don't overthink it

5. Output the email ready to send.

## Example Outputs

**Good Example 1 (referencing specific discussion):**
```
Subject: Great chatting about the design system challenges

Hi Sarah,

Thanks for walking me through Linear's approach to keyboard navigation — the way you've handled focus management across panels is exactly the kind of problem I love tackling.

Your question about how I'd handle the mobile constraints got me thinking. I sketched out a quick idea for the gesture-based approach we discussed — happy to share if helpful.

Looking forward to the next steps. Let me know if you need anything else from my side.

Best,
[Name]
```

**Good Example 2 (addressing a concern):**
```
Subject: Following up on our chat

Hi Marcus,

Thanks for the honest conversation about the team's pace. I appreciated you being direct about the 2-week sprint cycles.

You asked about my comfort with ambiguity in fast-moving environments. I should have mentioned — at [Company], we shipped weekly and I actually thrive in that environment. The constraints force prioritization, which is where good design happens.

Excited about the possibility of joining the team. Let me know what the next step looks like.

Best,
[Name]
```

**Good Example 3 (after portfolio review):**
```
Subject: Thanks for the portfolio feedback

Hi Jamie,

Thanks for the thoughtful questions about my MedRec project. Your pushback on the onboarding flow was spot on — in retrospect, I should have tested that assumption earlier.

The way you described Stripe's approach to design crits sounds like exactly the environment where I do my best work. I'd love to contribute to that culture.

Looking forward to hearing about next steps.

Best,
[Name]
```

**Good Example 4 (after whiteboard/design challenge):**
```
Subject: Thanks — and a revised take on the onboarding flow

Hi [Name],

Thanks for the design challenge today. The constraint you added mid-way (supporting offline mode) completely changed my approach — in a good way.

I kept thinking about it after and sketched a simpler solution. Attached if you're curious. Either way, I appreciated the realistic challenge.

Looking forward to hearing about next steps.

Best,
[Name]
```

**Good Example 5 (panel interview — multiple people):**
```
Subject: Thanks for the conversations today

Hi [Name],

Thanks for coordinating today's interviews. The conversations with [Person 1] about design systems and [Person 2] about research ops gave me a much clearer picture of the team's challenges.

[Person 1]'s question about token architecture stuck with me — I have some thoughts on the migration approach that might be useful. Happy to share.

Appreciate everyone's time. Looking forward to next steps.

Best,
[Name]
```

**Bad Examples (don't do this):**
```
❌ "Thank you so much for taking the time to meet with me today. I really enjoyed our conversation and learning more about the role. I'm very excited about the opportunity..."

❌ "I wanted to follow up and reiterate my strong interest in the position. I believe my skills and experience make me an excellent candidate..."
```

## Notes

- Reference something SPECIFIC — a comment, question, or insight from the conversation
- Keep it short — they're busy
- If you have something to share (sketch, article, resource), offer it
- If there was a concern, address it briefly and confidently
- Don't oversell — you already interviewed, now just be human
