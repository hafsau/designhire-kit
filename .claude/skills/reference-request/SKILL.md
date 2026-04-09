# Reference Request

Generate personalized emails to request professional references from past managers, colleagues, or clients.

## Usage

```
/reference-request
```

Then provide details about who you're asking and the role you're applying for.

## What It Does

1. Generates a personalized reference request email
2. Provides context they need to give a strong reference
3. Creates a follow-up thank-you template
4. Guides timing and reference management

## Why This Matters

- **Strong references close offers** — they're often the final checkpoint
- **Bad reference requests hurt you** — vague asks lead to vague references
- **Preparation makes references better** — giving context helps them advocate for you
- **Most designers underuse client references** — freelance/agency work = great references

## Instructions for Claude

When the user runs `/reference-request`:

### Phase 1: Context Gathering

1. Read context files:
   - `context/resume.md` for work history
   - `context/portfolio.md` for projects to reference
   - `context/writing-style.md` for tone

2. Ask for:
   - Who they're asking (name, their role when you worked together)
   - Your relationship (manager, colleague, client, mentor)
   - When you worked together and on what
   - The role you're applying for (company, title)
   - Specific skills/qualities you want them to highlight
   - Timeline (when references will be contacted)

### Phase 2: Generate Request

3. Create reference request email:

**Structure:**
- **Reconnect**: Brief personal touch if you haven't spoken recently
- **The Ask**: Clear request for a reference
- **Context**: The role and why you're excited about it
- **Help Them**: Specific talking points they can use
- **Logistics**: Timeline and how they'll be contacted
- **Easy Out**: Give them a graceful way to decline

**Tone:**
- Warm and appreciative
- Specific about what you need
- Respectful of their time
- Professional but not stiff

### Phase 3: Reference Brief

4. Create a "Reference Brief" they can use:

```
## Reference Brief for [Your Name]

**Role I'm applying for:** [Title] at [Company]

**Why I'm excited:** [1-2 sentences about the role]

**What they're looking for:**
- [Key requirement 1]
- [Key requirement 2]
- [Key requirement 3]

**Projects we worked on together:**
- [Project 1]: [Brief description + your role]
- [Project 2]: [Brief description + your role]

**Talking points (things you could mention):**
- [Specific skill/quality + example]
- [Specific skill/quality + example]
- [Specific skill/quality + example]

**Timeline:** They may contact you [timeframe]

**Contact method:** [Phone/email, whatever they prefer]
```

### Phase 4: Output

5. Output:
   - Personalized reference request email
   - Reference brief document
   - Thank-you template for after

## Reference Request Templates

### For a Former Manager
```
Subject: Would you be a reference for me?

Hi [Name],

I hope you're doing well. [Optional: Brief personal touch — "Congrats on the new role" or "Saw your post about X"]

I'm applying for a [Role] at [Company] and wondered if you'd be willing to be a reference. The role focuses on [brief description], and I think my work on [Project] with you would be directly relevant.

If you're open to it, I can send over some talking points and details about what they're looking for. I'd also be happy to jump on a quick call if that's easier.

No pressure if you're too busy — I completely understand.

Thanks so much,
[Your name]
```

### For a Former Colleague
```
Subject: Reference request

Hi [Name],

Hope things are going well at [their company/situation].

I'm in the final stages for a [Role] at [Company], and they're asking for references. Given how closely we worked on [Project], I thought you'd have great perspective on my [collaboration style / specific skill].

Would you be comfortable being a reference? I can share details about the role and some talking points if helpful.

Let me know — and no worries if the timing doesn't work.

Thanks,
[Your name]
```

### For a Client (Freelance/Agency)
```
Subject: Quick favor — reference for a design role

Hi [Name],

I hope this finds you well. It was great working with you on [Project] — I still think about [specific positive outcome or moment].

I'm applying for a [Role] at [Company] and they're asking for references. Since you saw my work firsthand on [Project], would you be willing to speak to that experience?

I can send over some context about the role and specific things that would be helpful to mention. Totally understand if you're not able to — I know you're busy.

Thanks for considering,
[Your name]
```

### For a Mentor (Non-Work Relationship)
```
Subject: Would you speak on my behalf?

Hi [Name],

I've appreciated your guidance over the past [timeframe], and I'm reaching out with a request.

I'm applying for a [Role] at [Company], and they're asking for character references. Given our conversations about [topic] and your insight into my growth as a designer, I thought you might have valuable perspective.

Would you be open to being a reference? I can share what the role involves and what would be most helpful to mention.

No pressure — and thank you either way for everything you've taught me.

[Your name]
```

## Reference Brief Example

```
## Reference Brief for Sarah Chen

**Role I'm applying for:** Senior Product Designer at Linear

**Why I'm excited:** Linear is building exactly the kind of complex, keyboard-first tool I love designing. Their approach to simplifying project management aligns with my work philosophy.

**What they're looking for:**
- Systems thinking and design system experience
- Ability to handle complex UX challenges
- Strong collaboration with engineering

**Projects we worked on together:**
- Stackflow Dashboard Redesign: I led the UX for the analytics dashboard overhaul. Reduced time-to-insight from 3 min to 30 sec.
- Design System Migration: I created the component architecture and led adoption across 3 product teams.

**Talking points (things you could mention):**
- My ability to simplify complex interfaces (Stackflow dashboard example)
- How I collaborate with engineers (you saw this firsthand in the design system work)
- My attention to edge cases and error states

**Timeline:** They may contact you in the next 1-2 weeks

**Contact method:** They'll likely email first, then schedule a call

**My contact:** sarah@email.com / 555-123-4567 if you have questions
```

## Follow-Up Templates

### After They Agree
```
Subject: Thanks — here's the reference brief

Hi [Name],

Thank you so much for agreeing to be a reference. I really appreciate it.

I've attached a brief with context about the role and some talking points. Feel free to use what's helpful and ignore what isn't — you know me better than a document can capture.

They'll likely reach out via [email/phone] in the next [timeframe]. Let me know if you have any questions.

Thanks again,
[Your name]
```

### After the Reference is Contacted
```
Subject: Thank you

Hi [Name],

I heard from [Company] that they spoke with you. Thank you so much for taking the time — I know how busy you are.

Whatever happens with this role, I really appreciate your support. I'll keep you posted on how it goes.

Thanks again,
[Your name]
```

### If You Get the Job
```
Subject: I got the job!

Hi [Name],

Wanted to let you know — I accepted the [Role] at [Company]! I'm sure your reference helped, and I'm really grateful.

Thank you for advocating for me. I'll keep you posted on how it goes.

[Your name]
```

### If You Don't Get the Job
```
Subject: Update on the role

Hi [Name],

Wanted to close the loop — I didn't end up getting the [Role] at [Company]. Disappointing, but I'm still glad I went for it.

Thank you so much for being a reference. I really appreciate your support, and I'll keep you in the loop as I continue the search.

[Your name]
```

## Timing & Logistics

**When to ask:**
- **2+ weeks before** references will be checked
- **After you're in final rounds** — don't waste their time on early stages
- **Not at the last minute** — gives them time to prepare

**Who to ask:**
- Former managers (strongest)
- Senior colleagues who saw your work closely
- Clients who can speak to outcomes
- Mentors (for character/growth references)

**How many:**
- Have **3-5 references ready**
- Companies typically ask for 2-3
- Mix of managers and peers is ideal

**Keeping references warm:**
- Check in every 6-12 months even when not job searching
- Share updates on your career
- Congratulate them on their wins
- Offer to be a reference for them

## What NOT to Do

- **Don't surprise them** — always ask before listing someone
- **Don't be vague** — "can you be a reference?" without context
- **Don't use outdated contacts** — 5+ years ago is stale unless you've stayed in touch
- **Don't skip the thank-you** — even if you don't get the job
- **Don't list references who'll give lukewarm endorsements** — better to have fewer strong ones
- **Don't forget to prep them** — the reference brief makes them better advocates

## Notes

- **Make it easy for them** — the more context you give, the stronger the reference
- **Former clients count** — designers often forget client references
- **Check in regardless** — use job search as excuse to reconnect
- **Quality over quantity** — 2 strong references beat 4 lukewarm ones
- **Close the loop** — always update them on outcome
