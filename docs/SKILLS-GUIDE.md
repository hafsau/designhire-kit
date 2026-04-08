# Skills Guide

How to use each skill in DesignHire Kit.

---

## Quick Reference

| Skill | When to Use | What You Need |
|-------|-------------|---------------|
| `/cover-letter` | Applying to a job | Job description |
| `/linkedin-outreach` | Messaging hiring manager/recruiter | Person's name, role, company |
| `/application-answer` | Filling out application questions | The question(s) |
| `/company-research` | Preparing for interview or application | Company name |
| `/interview-prep` | Before an interview | Company, role, job description, interview stage |
| `/thank-you` | After an interview | Interviewer name, what you discussed |

---

## /cover-letter

**Purpose:** Generate a portfolio-aware cover letter tailored to a specific job.

**When to use:** When you're ready to apply and need a cover letter that connects your work to their needs.

**How to use:**
1. Run `/cover-letter`
2. Paste the full job description when prompted
3. Claude generates a 3-4 paragraph cover letter

**What Claude does:**
- Reads your `context/resume.md` and `context/portfolio.md`
- Identifies which of your projects match their requirements
- Writes a cover letter that leads with fit, not generic enthusiasm
- Includes specific metrics from your portfolio

**Tips:**
- The more detailed your portfolio.md, the better the output
- If output seems generic, add more case study details
- Always review and personalize before sending

---

## /linkedin-outreach

**Purpose:** Write a short, personal LinkedIn message to a hiring manager or recruiter.

**When to use:** After applying, to get your application noticed. Or to network before applying.

**How to use:**
1. Run `/linkedin-outreach`
2. Provide: person's name, their role, the company, and the job you applied for
3. Optionally mention something specific about them or the company's design work
4. Claude generates a 3-5 sentence message

**What Claude does:**
- Reads your context files
- Creates a message that references their work or the company
- Connects to your relevant experience
- Ends with a soft ask, not a hard sell

**Tips:**
- Research the person first — a specific reference makes the message stand out
- Keep it short — recruiters skim
- Don't send immediately after applying; give it a day

**What NOT to say:**
- "I hope this finds you well"
- "I'd love to pick your brain"
- "I'm passionate about..."

---

## /application-answer

**Purpose:** Answer common application questions with specific, portfolio-backed responses.

**When to use:** When an application asks questions like "Why do you want to work here?" or "Tell us about a time you..."

**How to use:**
1. Run `/application-answer`
2. Paste the question(s) you need to answer
3. Claude generates answers using your portfolio

**What Claude does:**
- Analyzes what the question is really asking
- Finds relevant experience from your portfolio
- Structures answers using STAR method (but leads with result)
- Keeps answers to appropriate length (usually 150-300 words)

**Common question types it handles:**
- "Tell me about a time you..."
- "Why do you want to work here?"
- "What's your design process?"
- "Describe a challenge you faced..."
- "Why are you leaving your current role?"

**Tips:**
- Give Claude the word limit if specified
- If you have company context (from `/company-research`), mention it
- Edit for your voice — Claude gets you 80% there

---

## /company-research

**Purpose:** Research a company's design work, culture, and what they value.

**When to use:** Before writing a cover letter, before an interview, or when deciding whether to apply.

**How to use:**
1. Run `/company-research`
2. Provide: company name, optionally the role you're applying for
3. Claude researches and compiles a brief

**What Claude does:**
- Searches for their design team, leadership, principles
- Finds their design system, recent work, blog posts, talks
- Identifies what they value based on job descriptions and content
- Surfaces talking points and questions to ask
- Notes potential concerns or red flags

**Output includes:**
- Design team size and structure
- Key design leadership
- Recent design updates or launches
- Technology and tools they use
- What they emphasize in job posts
- Specific talking points for your application

**Tips:**
- Save the research output — reference it for cover letter and interview
- Look for specifics you can mention ("I noticed your recent redesign of...")
- Note their language — mirror it in your application

---

## /interview-prep

**Purpose:** Prepare for an interview with likely questions, talking points, and portfolio presentation guidance.

**When to use:** Before any interview — phone screen, portfolio review, onsite.

**How to use:**
1. Run `/interview-prep`
2. Provide: company name, role title, job description, interview stage
3. Claude generates a comprehensive prep guide

**What Claude does:**
- Reads your resume and portfolio
- Generates likely questions based on the job description
- Creates talking points that connect your work to their needs
- Recommends which case studies to present and how
- Suggests questions to ask them

**Output includes:**

**Likely Questions:**
- Based on job description requirements
- Common design interview questions
- Company-specific questions

**Talking Points:**
- For each key requirement, which of your projects demonstrates it
- Specific metrics to mention
- How to frame your experience

**Portfolio Presentation:**
- Which 2-3 case studies to lead with
- What to emphasize vs. skip
- How long to spend on each
- How to connect to their problems

**Questions to Ask Them:**
- Thoughtful, research-backed questions
- About the team, challenges, the role's impact

**Tips:**
- Run this the day before, not the morning of
- Practice your talking points out loud
- Have backup case studies ready if they ask for more

---

## /thank-you

**Purpose:** Write a post-interview thank you email that stands out.

**When to use:** Within 24 hours of an interview. Same day is ideal.

**How to use:**
1. Run `/thank-you`
2. Provide: interviewer's name and role, what you discussed, anything specific that came up, any concerns or timeline mentioned
3. Claude generates a ready-to-send email

**What Claude does:**
- References something specific from your conversation
- Reinforces why you're a good fit
- Addresses any concerns that came up
- Keeps it short (4-6 sentences)

**Tips:**
- Don't overthink it — short and specific beats long and generic
- If something came up you want to follow up on, mention it
- If you forgot to say something important, briefly add it

**What NOT to say:**
- "Thank you for your time" (generic)
- "I really enjoyed our conversation" (empty)
- Long paragraphs restating your qualifications

---

## Skill Combinations

### Applying to a job (full workflow):
1. `/company-research` — understand what they value
2. `/cover-letter` — write the application
3. `/linkedin-outreach` — message the hiring manager
4. `/application-answer` — if there are additional questions

### Preparing for an interview:
1. `/company-research` — if you haven't already
2. `/interview-prep` — generate questions and talking points
3. Practice out loud
4. `/thank-you` — after the interview

---

## Improving Output Quality

If output seems generic or off:

1. **Add more detail to context files** — especially portfolio.md
2. **Include metrics** — "improved" is vague, "reduced by 35%" is concrete
3. **Add writing samples** — to writing-style.md so Claude learns your voice
4. **Be specific in prompts** — tell Claude what you want emphasized

Remember: Claude is a starting point. Always review and personalize before sending.
