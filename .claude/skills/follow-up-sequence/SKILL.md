# Follow-Up Sequence

Generate a structured follow-up plan after applying to a job.

## Usage

```
/follow-up-sequence
```

Then provide details about the application.

## What It Does

1. Creates a day-by-day follow-up plan
2. Writes ready-to-send messages for each touchpoint
3. Adapts based on company size and role level
4. Tells you when to stop following up

## Instructions for Claude

When the user runs `/follow-up-sequence`:

1. Read context files:
   - `context/resume.md` for name and background
   - `context/portfolio.md` for relevant projects to reference
   - `context/writing-style.md` for tone

2. **Check if context files are filled in.** If they contain placeholder text, ask for the user's name and a brief background.

3. Ask for:
   - Company name
   - Role applied for
   - How they applied (website, referral, email, LinkedIn)
   - Hiring manager or recruiter name (if known)
   - Any connections at the company
   - Date of application

4. Generate a follow-up sequence:

### Day-by-Day Plan

```
# Follow-Up Sequence: [Role] at [Company]

Applied: [Date]

## Day 0 (Application Day)
Action: Save the job description (it may be taken down)
Notes: Record who posted it, any names mentioned

## Day 1-2: LinkedIn Outreach
Action: Message the hiring manager or recruiter
Who to contact: [Name/role or how to find them]
Message: [Ready-to-send message]

## Day 3-5: Wait
Action: None — give them time to see your application
Watch for: Profile views, connection requests

## Day 7: Email Follow-Up (if you have email)
Action: Send a brief follow-up email
Only if: You have a direct email address
Message: [Ready-to-send email]

## Day 10-14: Final Check-In
Action: One last message if no response
Only if: You haven't heard anything
Message: [Ready-to-send message]

## After Day 14: Move On
Action: Assume no response means no (for now)
Don't: Send more messages
Do: Keep applying elsewhere; they may resurface later
```

### Ready-to-Send Messages

**Day 1-2 LinkedIn Message:**

```
Hi [Name] — I applied for the [Role] at [Company] [today/yesterday].

[One sentence connecting your experience to their needs or referencing their work].

[Soft ask — not demanding].

[Your name]
```

**Day 7 Email (if applicable):**

```
Subject: Following up — [Role] application

Hi [Name],

I applied for the [Role] last week and wanted to make sure it came through.

[One new piece of value — insight, relevant work, or connection to their recent news].

Happy to answer any questions about my background.

Best,
[Your name]
```

**Day 10-14 Final Message:**

```
Hi [Name] —

Just checking in on the [Role]. I'm still very interested, but I understand if the timing isn't right or you've moved forward with other candidates.

If it would help, I'm happy to share [specific thing — portfolio walkthrough, quick call, etc.].

Either way, thanks for your time.

[Your name]
```

### Adjustments by Scenario

**If you have a referral:**
- Mention the referral in Day 1-2 message
- Ask your referral to nudge after Day 5 if no response
- Your messages can be shorter — the referral does the heavy lifting

**If it's a startup (<50 people):**
- Faster timeline — compress to Day 1, Day 4, Day 7
- More casual tone
- Founder might be the hiring manager

**If it's enterprise (1000+ people):**
- Slower timeline — extend to Day 3, Day 10, Day 17
- More formal tone
- Expect to talk to recruiters first, not hiring managers

**If you applied through an ATS:**
- Harder to follow up — focus on finding a person to contact
- LinkedIn is your best bet
- Check if anyone in your network knows someone there

### What NOT to Do

```
DON'T:
- Follow up more than 3 times total
- Send the same message twice
- Sound desperate or passive-aggressive
- Follow up on weekends
- CC multiple people at the company
- Use "just checking in" as your entire message

If no response after Day 14:
- They're not interested right now
- Don't burn the bridge — you may apply again
- Move on mentally, but leave the door open
```

5. Output the complete sequence with all messages ready to copy.

## Example Output

```
# Follow-Up Sequence: Senior Product Designer at Linear

Applied: Monday, April 7

---

## Day 0 (Monday)
✓ Saved job description
✓ Noted: Posted by Karri Saarinen (CEO/Co-founder)

---

## Day 1-2 (Tuesday-Wednesday): LinkedIn Outreach

Target: Karri Saarinen or a design lead at Linear

LinkedIn Message:
```
Hi Karri — I applied for the Senior Product Designer role yesterday.

I've been a Linear user for 2 years, and your recent mobile app release got me thinking about the interaction design challenges of keyboard-first on mobile. I tackled something similar at Stackflow — would love to chat about it.

Sarah
```

---

## Day 3-5 (Thursday-Saturday): Wait

No action. Watch for:
- LinkedIn profile views
- Connection requests
- Email responses

---

## Day 7 (Next Monday): Email Follow-Up

Only if: You found an email address (try karri@linear.app or check their team page)

Email:
```
Subject: Following up — Senior Product Designer

Hi Karri,

I applied for the Senior Product Designer role last week. Since then, I've been thinking about the dashboard redesign you mentioned in your recent blog post.

I did something similar at Stackflow — took a "powerful but overwhelming" analytics tool and made it actually usable. Time-to-insight dropped from 3 minutes to 30 seconds. I'd love to share how.

Happy to chat if the timing works.

Best,
Sarah Chen
```

---

## Day 10-14 (Thursday-Monday): Final Check-In

Only if: No response to anything

LinkedIn Message:
```
Hi Karri —

Just checking in on the Senior Product Designer role. Still interested, but I understand if you've moved forward or the timing isn't right.

If it helps, happy to do a quick portfolio walkthrough. Either way, I appreciate your time.

Sarah
```

---

## After Day 14: Move On

- Stop messaging
- Keep using Linear (they may notice engaged users)
- Check back in 2-3 months if they post the role again
- Don't take it personally — they get hundreds of applications

---

## Notes for This Application

- Linear is a small team (~50) — faster decisions, so shorter timeline is fine
- Karri is active on Twitter — could engage with his posts (genuinely, not sycophantically)
- Strong design culture — they'll notice if you're a real user
```

## Notes

- Always leave at least 2-3 days between messages
- Never sound desperate or passive-aggressive
- Include something of value in each message (not just "checking in")
- Know when to stop — 3 touches maximum
- Adjust timeline based on company size and culture
- If you have a referral, use it
