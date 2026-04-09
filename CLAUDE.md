# DesignHire Kit — Claude Code Skills for Designers

**Version:** 0.1.0-beta

A collection of Claude Code skills to automate your job search. Portfolio-aware, humanized, designer-first.

---

## Your Context Files

Before using the skills, fill in these files in the `context/` folder:

1. **context/resume.md** — Your full resume text
2. **context/portfolio.md** — Case studies with metrics
3. **context/writing-style.md** — Your voice and tone preferences
4. **context/target-companies.md** — Dream companies to track

---

## Quick Start

1. Fill in your context files
2. Paste a job description
3. Run a skill: `/cover-letter`, `/linkedin-outreach`, etc.

---

## Humanizer Guidelines

When generating content, ALWAYS follow these rules to sound human, not AI:

### Content Patterns to AVOID
- Inflated significance claims ("This marks a pivotal moment...")
- Name-dropping credentials unnecessarily
- Superficial "-ing" phrases ("leveraging," "revolutionizing")
- Flowery promotional language
- Vague attributions ("experts say," "studies show")
- Formulaic problem-solution structures

### Language Patterns to AVOID
- Overused AI vocabulary: "testament," "landscape," "delve," "tapestry," "multifaceted," "pivotal," "nuanced," "robust," "leverage," "synergy," "paradigm"
- Awkward verb avoidance ("serves as" instead of "is")
- Synonym cycling (saying the same thing 3 different ways)
- False conceptual ranges ("from X to Y")
- Excessive passive voice

### Style Patterns to AVOID
- Em dash overuse (—)
- Excessive boldface
- Title Case On Every Word
- Emojis in professional content
- Hyphenated compound words unnecessarily

### Communication Patterns to AVOID
- Chatbot closing phrases ("Feel free to reach out!")
- Sycophantic tone ("Great question!")
- Generic conclusions ("I look forward to hearing from you")
- Meta-signposting ("In this letter, I will...")
- Persuasive tropes ("At its core...")

### Designer-Specific Patterns to AVOID
These are phrases AI uses when trying to sound like a designer:

**Fake humility:**
- "I had the privilege of..." (just say "I worked on")
- "I was fortunate to..." (just say what you did)
- "I humbly believe..." (just state your opinion)

**Buzzword soup:**
- "Human-centered design thinking methodologies"
- "Holistic user experience ecosystem"
- "Design-driven innovation framework"
- "Cross-functional collaborative synergies"

**Vague impact claims:**
- "Significantly improved the user experience"
- "Made a meaningful impact on the product"
- "Drove engagement and satisfaction"
- (Always use specific metrics instead)

**Process theater:**
- "After extensive stakeholder alignment sessions..."
- "Through rigorous design thinking workshops..."
- "Following comprehensive user research phases..."
- (Just describe what you actually did)

**Emotional overselling:**
- "I'm incredibly passionate about..."
- "I'm deeply committed to..."
- "I'm extremely excited about the opportunity..."
- (Show passion through specifics, not adjectives)

### What TO DO Instead
- Be specific and direct
- Use first person naturally ("I built..." not "The designer built...")
- Vary sentence length and rhythm
- Reference actual projects and metrics from portfolio
- Allow controlled messiness — not every sentence needs to be perfect
- Have opinions and personality
- End with specific call to action, not generic phrases

---

## Designer Voice Guidelines

### Tone
- Confident but not arrogant
- Specific, not vague
- Portfolio-aware (reference actual work)
- Conversational but professional

### Structure
- Lead with what matters most
- Connect your work to their problems
- Use metrics when available (e.g., "reduced error rates by 35%")
- End with clear next step

### Examples

**Bad (AI-sounding):**
> "I am writing to express my enthusiastic interest in the Product Designer position at your esteemed organization. Throughout my multifaceted career journey, I have consistently demonstrated a robust commitment to leveraging design thinking methodologies..."

**Good (Human):**
> "I saw the Product Designer role at Acme and got excited — you're building exactly the kind of complex B2B tool I love working on. My recent project, MedRec, was a diabetes management app where I reduced error rates by 35% by simplifying a workflow that was overwhelming users..."

**Bad LinkedIn message:**
> "Dear Hiring Manager, I hope this message finds you well. I wanted to reach out regarding the exciting opportunity at your company..."

**Good LinkedIn message:**
> "Hi Sarah — I just applied for the Design Engineer role. I noticed you recently shipped the new dashboard redesign. The card sorting approach you used is similar to what I did on my healthcare app. Would love to chat about how you handled the data density problem."

---

## Available Skills

| Skill | Command | Description |
|-------|---------|-------------|
| Cover Letter | `/cover-letter` | Portfolio-aware cover letter from job description |
| Resume Tailor | `/resume-tailor` | Customize resume for specific role with ATS optimization |
| LinkedIn Outreach | `/linkedin-outreach` | Message to hiring manager or recruiter |
| Application Answers | `/application-answer` | Answer common application questions |
| Company Research | `/company-research` | Research company's design work and culture |
| Interview Prep | `/interview-prep` | Generate likely questions and talking points |
| Thank You Email | `/thank-you` | Post-interview follow-up |
| Portfolio Pitch | `/portfolio-pitch` | Tailor portfolio presentation for specific company |
| Follow-Up Sequence | `/follow-up-sequence` | Day-by-day follow-up plan after applying |
| Informational Interview | `/informational-interview` | Reach out to designers at target companies |
| Reference Request | `/reference-request` | Request references from past managers/colleagues |
| Networking Outreach | `/networking-outreach` | Build genuine professional relationships |

---

## Saving Outputs

When generating cover letters, resumes, or other application materials:

1. **Save to the `applications/` folder** organized by company:
   ```
   applications/
   ├── linear/
   │   ├── cover-letter.md
   │   ├── resume.md
   │   └── notes.md
   ├── figma/
   │   └── ...
   ```

2. **Convert to PDF before submitting** (formatting matters):
   ```bash
   # Install pandoc once
   brew install pandoc

   # Convert any .md to .pdf
   pandoc cover-letter.md -o cover-letter.pdf
   ```

3. **Always save as files** — don't just display in terminal. Ask Claude to save outputs to `applications/[company-name]/`

---

## Tips for Best Results

1. **Be specific in your context files** — The more details, the better output
2. **Include metrics** — Numbers make your work concrete
3. **Name your case studies** — Reference them by name, not "a project"
4. **Update regularly** — Keep context files current
5. **Edit the output** — AI is a starting point, not final draft
6. **Save and convert to PDF** — Terminal output isn't submittable
