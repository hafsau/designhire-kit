# DesignHire Kit

A Claude Code starter kit that automates your designer job search. Portfolio-aware cover letters, LinkedIn outreach, interview prep, and more.

## What's Included

**12 Skills:**
- `/cover-letter` — Generate portfolio-backed cover letters from job descriptions
- `/resume-tailor` — Customize your resume for specific roles with ATS optimization
- `/linkedin-outreach` — Write short, personal messages to hiring managers
- `/application-answer` — Answer common application questions with real examples
- `/company-research` — Research a company's design work and culture
- `/interview-prep` — Prepare questions, talking points, and portfolio presentation
- `/thank-you` — Post-interview follow-up emails that reference your conversation
- `/portfolio-pitch` — Tailor your portfolio presentation for a specific company
- `/follow-up-sequence` — Day-by-day follow-up plan after applying
- `/informational-interview` — Reach out to designers at target companies
- `/reference-request` — Request references from past managers/colleagues
- `/networking-outreach` — Build genuine professional relationships

**Context Templates:**
- Resume, portfolio, writing style, and target companies templates
- Fill these in once, use across all skills

**Humanizer Guidelines:**
- Built-in rules to avoid AI-sounding output
- Your content sounds like you, not a chatbot

## Setup

### Prerequisites

- [Claude Code](https://claude.ai/code) installed
- Claude Pro or Team subscription

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/hafsau/designhire-kit.git
   cd designhire-kit
   ```

2. **Fill in your context files** in the `context/` folder:
   - `resume.md` — Your full resume
   - `portfolio.md` — Case studies with metrics
   - `writing-style.md` — Your voice and tone preferences
   - `target-companies.md` — Companies you're targeting (optional)

3. **Start Claude Code:**
   ```bash
   claude
   ```

4. **Verify skills are loaded:**
   ```
   /skills
   ```
   You should see all 12 skills listed.

## Usage

### Generate a Cover Letter

```
/cover-letter
```

Paste the job description when prompted. Claude will read your context files and generate a personalized cover letter.

### Research a Company

```
/company-research
```

Provide the company name. Get a brief on their design team, recent work, and talking points for your application.

### Prepare for an Interview

```
/interview-prep
```

Provide the company, role, and job description. Get likely questions, talking points, and portfolio presentation guidance.

## File Structure

```
designhire-kit/
├── CLAUDE.md              # Master context + humanizer rules
├── .claude/skills/        # Skill definitions (12 total)
│   ├── cover-letter/
│   ├── resume-tailor/
│   ├── linkedin-outreach/
│   ├── application-answer/
│   ├── company-research/
│   ├── interview-prep/
│   ├── thank-you/
│   ├── portfolio-pitch/
│   ├── follow-up-sequence/
│   ├── informational-interview/
│   ├── reference-request/
│   └── networking-outreach/
├── context/               # Your info (edit these)
│   ├── resume.md
│   ├── portfolio.md
│   ├── writing-style.md
│   └── target-companies.md
├── templates/             # Reference templates
└── docs/                  # Full documentation
```

## Tips for Best Results

1. **Be specific in context files** — Include metrics, project names, and concrete details
2. **Update regularly** — Keep your portfolio.md current
3. **Edit the output** — Claude gets you 80% there; add your personal touch
4. **Test with real jobs** — The more you use it, the better you'll tune your context

## Documentation

- [Setup Guide](docs/SETUP.md) — Detailed installation instructions
- [Skills Guide](docs/SKILLS-GUIDE.md) — How to use each skill
- [FAQ](docs/FAQ.md) — Common questions and troubleshooting

## License

MIT
