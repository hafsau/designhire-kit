# Setup Guide

Get DesignHire Kit running in 5 minutes.

---

## Prerequisites

- **Claude Code** installed and working ([Get it here](https://claude.ai/code))
- A Claude subscription (Pro or Team)
- Basic familiarity with running terminal commands

---

## Installation

### Step 1: Download the Kit

Download and unzip the DesignHire Kit to a folder on your computer. You can put it anywhere — your Documents folder, Desktop, or a dedicated projects folder.

```
~/Documents/designhire-kit/
```

### Step 2: Open in Claude Code

Open Claude Code and navigate to your kit folder:

```bash
cd ~/Documents/designhire-kit
claude
```

Or open Claude Code and use the `/cd` command to navigate to your folder.

### Step 3: Verify Installation

Run this command to confirm Claude can see the skills:

```
/skills
```

You should see:
- `/cover-letter`
- `/linkedin-outreach`
- `/application-answer`
- `/company-research`
- `/interview-prep`
- `/thank-you`

If you see these, you're set up correctly.

---

## Configure Your Profile

Before using the skills, fill in your context files. These provide the background Claude uses to personalize your content.

### Required Files

Open each file and replace the placeholder text with your information:

1. **`context/resume.md`**
   - Your full resume
   - Experience, skills, education
   - What you're looking for

2. **`context/portfolio.md`**
   - 3-5 case studies with metrics
   - What you did, key decisions, results
   - Tags for matching to job requirements

3. **`context/writing-style.md`**
   - Your tone and voice preferences
   - Words you use vs. avoid
   - Sample writing for Claude to learn from

4. **`context/target-companies.md`** (optional but helpful)
   - Dream companies list
   - Industries you're targeting
   - Company criteria

### Tips for Good Context Files

- **Be specific** — "Reduced error rates by 35%" beats "Improved the product"
- **Include metrics** — Numbers make your work concrete
- **Be honest** — Don't exaggerate; Claude will reference this directly
- **Update regularly** — Keep these current as your experience grows

---

## Your First Skill

Let's test with a cover letter:

1. Find a job posting you're interested in
2. Run `/cover-letter`
3. When prompted, paste the job description
4. Claude will generate a cover letter using your context

If it doesn't reference your portfolio or sounds generic, your context files may need more detail.

---

## Folder Structure

```
designhire-kit/
├── CLAUDE.md              # Master context + humanizer rules (don't edit)
├── .claude/
│   └── skills/            # Skill definitions (don't edit)
│       ├── cover-letter/
│       ├── linkedin-outreach/
│       ├── application-answer/
│       ├── company-research/
│       ├── interview-prep/
│       └── thank-you/
├── context/               # YOUR INFO (edit these)
│   ├── resume.md
│   ├── portfolio.md
│   ├── writing-style.md
│   └── target-companies.md
├── templates/             # Reference templates
└── docs/                  # Documentation
    ├── SETUP.md           # This file
    ├── SKILLS-GUIDE.md    # How to use each skill
    └── FAQ.md             # Common questions
```

---

## Troubleshooting

### "Skills not showing up"

- Make sure you're in the designhire-kit folder when you run Claude Code
- Check that `.claude/skills/` exists and has the SKILL.md files
- Try restarting Claude Code

### "Output sounds generic/AI-like"

- Your context files are probably too sparse
- Add more detail to `context/portfolio.md` — specific projects, metrics, decisions
- Add writing samples to `context/writing-style.md`

### "Claude isn't reading my context files"

- Make sure files are in the `context/` folder (not elsewhere)
- Check that files are saved (not just open in editor)
- File names must match exactly: `resume.md`, `portfolio.md`, etc.

### "Skill errors out"

- Check Claude Code is up to date
- Try running a simpler skill first (`/thank-you`)
- If persistent, check the skill's SKILL.md file for issues

---

## Updating the Kit

When updates are released:

1. Download the new version
2. **Don't overwrite your `context/` folder** — this has your personal info
3. Replace everything else (skills, docs, templates)
4. Check the changelog for new skills or changes

---

## Getting Help

- Check `docs/FAQ.md` for common questions
- Join our Discord for community support
- Email support@[your-domain].com for direct help

---

## Next Steps

1. Fill in your context files
2. Read `docs/SKILLS-GUIDE.md` to understand each skill
3. Try `/cover-letter` with a real job posting
4. Iterate on your context files based on output quality
