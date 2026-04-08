# Frequently Asked Questions

---

## Setup & Installation

### Do I need an API key?
No. You use your existing Claude subscription (Pro or Team). No additional API keys required.

### Does this work on Windows?
Yes. Claude Code works on Mac, Windows, and Linux. The skills work the same on all platforms.

### Do I need to know how to code?
No. You just need to be comfortable running basic terminal commands and editing text files.

### Can I use this with other Claude Code projects?
Yes. You can copy the `.claude/skills/` folder and `CLAUDE.md` to any project. Just make sure your `context/` files are accessible.

---

## Using the Skills

### Why does my output sound generic?
Your context files probably need more detail. Add:
- Specific metrics to your portfolio case studies
- More case studies (aim for 3-5)
- Writing samples to writing-style.md

### Can I edit the skill files?
Yes, they're just markdown. But be careful — changing the structure might break them. The `context/` files are where you should customize.

### How do I add my own skills?
Create a new folder in `.claude/skills/` with a `SKILL.md` file. Follow the same format as the existing skills.

### Why isn't Claude reading my context files?
- Make sure you're running Claude Code from the designhire-kit folder
- Check file names match exactly (resume.md, not Resume.md)
- Make sure files are saved, not just open in an editor

### Can I use this for non-design jobs?
The skills are designed for designers, but the structure works for any job search. You'd want to edit the prompts in the skill files and CLAUDE.md to fit your field.

---

## Privacy & Security

### Where does my data go?
Everything stays on your computer. The context files are only read by Claude when you run a skill. Nothing is uploaded or stored externally.

### Is it safe to put my resume in these files?
As safe as any file on your computer. The files are plain text. They're not sent anywhere except to Claude when you run a skill.

### Does this store my job applications?
No. The kit doesn't track or store anything. You'll need your own system (spreadsheet, Notion, etc.) to track applications.

---

## Output Quality

### The cover letter doesn't mention my best project. Why?
Claude matches projects to job requirements. If a project isn't mentioned, either:
- It wasn't relevant to this specific job
- The case study in portfolio.md doesn't clearly show the connection
- Add tags to your case studies to help Claude match them

### How do I make output sound more like me?
Fill out `context/writing-style.md` thoroughly:
- Add 2-3 samples of your actual writing
- List words you use and words you avoid
- Describe your tone

### Should I send Claude's output directly?
No. Always review and edit. Claude gets you 80% there; you add the human touch.

---

## Troubleshooting

### Skills don't show up when I run /skills
- Make sure you're in the designhire-kit folder
- Check `.claude/skills/` exists with SKILL.md files in each subfolder
- Try restarting Claude Code

### Claude errors out when running a skill
- Check Claude Code is up to date
- Try a simpler skill first (/thank-you)
- Check the SKILL.md file for formatting issues

### Output is cut off or incomplete
- Some skills generate long output; give Claude time
- If persistent, try breaking your request into smaller parts

---

## Updates & Support

### How do I get updates?
Check the download page for new versions. Back up your `context/` folder before updating.

### Something's broken. Where do I get help?
- Check this FAQ
- Open an issue on GitHub: https://github.com/hafsau/designhire-kit/issues
- Email for direct help (see README for contact)

### Can I request new skills?
Yes! Let us know what would help your job search. Common requests may become new skills.

---

## General

### How is this different from ChatGPT?
This is built specifically for Claude Code, with skills that reference your portfolio and writing style. ChatGPT can write cover letters, but it doesn't have your context built in.

### Why Claude Code instead of a web app?
- No API key management
- Your data stays local
- Integrates with your workflow
- Skills can evolve with Claude's capabilities

### Is there a free tier?
The kit is a one-time purchase. You need your own Claude subscription (Pro or Team) to use it.
