# Beta Test Plan

A structured 2-week beta test to validate and improve DesignHire Kit before launch.

---

## Goals

1. **Validate** — Do the skills produce usable output?
2. **Iterate** — What tweaks improve quality?
3. **Prove** — Collect evidence it works (interviews landed)
4. **Refine** — Add the "little tricks" that make the difference

---

## Beta Cohort

**Target: 10-15 designers actively job searching**

### Ideal Beta Testers
- Currently applying to jobs (not passively looking)
- Comfortable with command line / Claude Code
- Willing to give detailed feedback
- Mix of experience levels (junior, mid, senior)

### Where to Find Them
- [ ] Designer Slack communities (Designer Hangout, etc.)
- [ ] Twitter/X design community
- [ ] ADPList connections
- [ ] Personal network
- [ ] LinkedIn post

### Recruitment Message
```
Looking for 10-15 designers actively job hunting to beta test a Claude Code toolkit I built.

What it does:
- Generates portfolio-aware cover letters
- Writes LinkedIn outreach messages
- Preps you for interviews with company research

What I need from you:
- Use it for real applications over 2 weeks
- 15-min feedback call at the end
- Tell me what works and what's garbage

What you get:
- Free lifetime access
- Direct input on features
- Credit as a founding tester

DM if interested. Looking for people applying NOW, not "thinking about it."
```

---

## Beta Timeline

### Week 0: Setup (2-3 days)
- [ ] Recruit 10-15 testers
- [ ] Create private Discord/Slack channel for beta group
- [ ] Send onboarding instructions
- [ ] Collect baseline info (current application count, response rate)

### Week 1: Initial Usage
- [ ] Testers use kit for real applications
- [ ] Daily check-ins in Discord (what worked, what didn't)
- [ ] Collect raw outputs + feedback
- [ ] Make quick fixes based on obvious issues

### Week 2: Iteration + Results
- [ ] Push updated skills based on Week 1 feedback
- [ ] Testers continue using updated version
- [ ] Track interview requests received
- [ ] Conduct 15-min feedback calls

### Week 3: Analysis + Launch Prep
- [ ] Compile all feedback
- [ ] Final skill improvements
- [ ] Write case studies from successful testers
- [ ] Prepare launch materials

---

## Feedback Collection

### Daily Discord Check-In Prompts
```
Day 1: Which skill did you try first? Share the output (anonymized). What would you change?

Day 3: How many applications have you sent using the kit? Any responses yet?

Day 5: What's the most annoying thing about using the kit? What do you wish it did?

Day 7: Mid-point check: Would you recommend this to a friend? Why/why not?

Day 10: Any interviews scheduled? What do you think made the difference?

Day 14: Final day! Overall rating 1-10? What's the #1 improvement needed?
```

### Feedback Form (End of Beta)
```
1. How many applications did you submit using the kit? ___

2. How many responses/interviews did you get? ___

3. Which skill was most useful?
   [ ] /cover-letter
   [ ] /linkedin-outreach
   [ ] /application-answer
   [ ] /company-research
   [ ] /interview-prep
   [ ] /thank-you

4. Which skill needs the most work?
   [ ] Same options

5. Rate the output quality (1-10): ___

6. How much editing did outputs need?
   [ ] Ready to send as-is
   [ ] Minor tweaks (5 min)
   [ ] Significant editing (15+ min)
   [ ] Had to rewrite most of it

7. What's the #1 thing that would make this worth paying for?
   [Open text]

8. What "tricks" did you discover that improved outputs?
   [Open text]

9. Would you pay $49 for this? Why/why not?
   [Open text]

10. Can we use your feedback as a testimonial? (with or without name)
    [ ] Yes, with name
    [ ] Yes, anonymous
    [ ] No
```

### 15-Min Feedback Call Questions
1. Walk me through how you used the kit for a real application
2. Show me an output you actually sent — what did you change?
3. Show me an output that was unusable — what went wrong?
4. What's missing that would make this a no-brainer purchase?
5. If you got an interview, what do you think made the difference?

---

## Metrics to Track

### Quantitative
| Metric | Target |
|--------|--------|
| Applications sent using kit | 50+ total across testers |
| Response rate | >10% (industry avg is 2-5%) |
| Interviews landed | 5+ |
| Output usability (needs <5 min editing) | >70% |
| Would pay $49 | >60% of testers |

### Qualitative
- Common complaints (prioritize fixes)
- "Little tricks" discovered
- Best outputs (use as examples)
- Worst outputs (diagnose and fix)

---

## Iteration Process

### Quick Fixes (Same Day)
- Typos or obvious errors in skills
- Missing instructions causing confusion
- Broken functionality

### Weekly Updates
- Prompt improvements based on feedback
- New examples added to skills
- Edge case handling

### Post-Beta Improvements
- New skills requested by testers
- Major prompt overhauls
- Documentation updates

---

## Success Criteria

**Beta is successful if:**
- [ ] At least 5 testers get interview requests
- [ ] Average output quality rating ≥7/10
- [ ] >60% say they'd pay $49
- [ ] We identify 10+ specific improvements to make
- [ ] We have 3+ usable testimonials

**Beta fails if:**
- [ ] <3 testers complete the full 2 weeks
- [ ] Output quality rating <5/10
- [ ] 0 interviews from kit-generated materials
- [ ] Testers say it's not better than ChatGPT

---

## Onboarding Instructions for Testers

```
# Welcome to DesignHire Kit Beta

Thanks for testing! Here's how to get started.

## Setup (10 minutes)

1. Make sure you have Claude Code installed
   - If not: https://claude.ai/code

2. Clone the repo:
   git clone https://github.com/hafsau/designhire-kit.git
   cd designhire-kit

3. Fill in your context files in the `context/` folder:
   - resume.md — Your full resume
   - portfolio.md — 2-3 case studies with metrics
   - writing-style.md — Your tone preferences

4. Start Claude Code:
   claude

5. Test it works:
   /cover-letter
   (paste any job description)

## How to Give Feedback

- Join our Discord: [link]
- Post outputs (anonymize company names if needed)
- Tell us: what worked, what sucked, what you changed
- Be brutally honest — we need real feedback, not politeness

## What We're Testing

- Do outputs sound human or AI-generated?
- Do they reference your portfolio correctly?
- How much editing do they need?
- Do they actually get responses?

## Questions?

DM me or post in #beta-support

Thanks for helping make this better!
```

---

## Post-Beta Deliverables

After beta, we should have:

1. **Improved Skills** — Updated prompts based on real feedback
2. **Proof Points** — "X interviews from Y applications"
3. **Testimonials** — 3-5 quotes from real users
4. **Case Studies** — 1-2 detailed success stories
5. **FAQ Updates** — Real questions from real users
6. **Pricing Validation** — Confidence in $49 price point

---

## Notes

Use this space to track beta progress:

### Testers Recruited
| Name | Source | Start Date | Status |
|------|--------|------------|--------|
| | | | |

### Key Feedback Themes
| Theme | Frequency | Action |
|-------|-----------|--------|
| | | |

### Improvements Made
| Date | Change | Result |
|------|--------|--------|
| | | |
