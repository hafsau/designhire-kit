# Testing Checklist

Work through this checklist to verify all skills function correctly before launch.

---

## Setup Tests

### Context File Detection
- [ ] **Empty context test**: Reset context files to templates, run `/cover-letter`. Should prompt for info instead of using placeholders.
- [ ] **Partial context test**: Fill in only resume.md, run `/linkedin-outreach`. Should use resume but ask for missing portfolio info.
- [ ] **Full context test**: Fill in all context files, run any skill. Should use context without prompting.

---

## Skill Tests

### /cover-letter

**Test 1: B2B SaaS Role**
- [ ] Run `/cover-letter`
- [ ] Paste this job description:
```
Senior Product Designer at Linear

We're looking for a Senior Product Designer to join our team. You'll work on our core product, designing features that help teams move faster.

Requirements:
- 5+ years of product design experience
- Experience with complex B2B tools
- Strong systems thinking
- Comfortable working with engineers
- Experience with design systems
```
- [ ] Verify output:
  - [ ] References Linear specifically (not generic)
  - [ ] Mentions a portfolio project by name
  - [ ] Includes at least one metric
  - [ ] 250-400 words
  - [ ] No AI-giveaway phrases ("I am writing to express...")
  - [ ] Ends with specific call to action

**Test 2: Healthcare Role**
- [ ] Run `/cover-letter` with a healthcare job description
- [ ] Verify it leads with MedTrack/healthcare experience (not Stackflow)

**Test 3: Design Systems Role**
- [ ] Run `/cover-letter` with a role emphasizing design systems
- [ ] Verify it emphasizes the Medley design system case study

---

### /linkedin-outreach

**Test 1: Hiring Manager Message**
- [ ] Run `/linkedin-outreach`
- [ ] Input: "Sarah Chen, Design Lead at Figma" for "Senior Product Designer"
- [ ] Verify output:
  - [ ] 3-5 sentences max
  - [ ] References Figma or Sarah's work specifically
  - [ ] Mentions relevant portfolio experience
  - [ ] No "I hope this finds you well"
  - [ ] No "I'd love to pick your brain"
  - [ ] Soft ask at end

**Test 2: Recruiter Message**
- [ ] Run `/linkedin-outreach`
- [ ] Input: "Jamie Smith, Technical Recruiter at Stripe" for "Product Designer"
- [ ] Verify output adjusts tone for recruiter (less technical, more direct)

**Test 3: With Specific Reference**
- [ ] Run `/linkedin-outreach`
- [ ] Add specific info: "They just shipped a new dashboard redesign"
- [ ] Verify output references this specific work

---

### /application-answer

**Test 1: "Tell me about a time..." Question**
- [ ] Run `/application-answer`
- [ ] Paste: "Tell me about a time you had to convince stakeholders to change direction."
- [ ] Verify output:
  - [ ] Leads with the result, not backstory
  - [ ] References specific project
  - [ ] Includes metric or outcome
  - [ ] 200-300 words
  - [ ] Shows self-awareness

**Test 2: "Why do you want to work here?" Question**
- [ ] Run `/application-answer`
- [ ] Paste: "Why do you want to work at Notion?"
- [ ] Verify output is specific to Notion (not generic)

**Test 3: "What's your design process?" Question**
- [ ] Run `/application-answer`
- [ ] Paste: "Describe your design process."
- [ ] Verify output shows adaptability (not textbook process)

**Test 4: Multiple Questions**
- [ ] Run `/application-answer`
- [ ] Paste 3 questions at once
- [ ] Verify all 3 are answered and clearly labeled

**Test 5: Word Limit**
- [ ] Run `/application-answer`
- [ ] Paste: "Why are you interested in this role? (100 words max)"
- [ ] Verify output respects the word limit

---

### /company-research

**Test 1: Well-Known Company**
- [ ] Run `/company-research`
- [ ] Input: "Figma"
- [ ] Verify output includes:
  - [ ] Design team info
  - [ ] Recent design work
  - [ ] What they value
  - [ ] Talking points for application
  - [ ] Questions to ask
  - [ ] Red flags or concerns

**Test 2: Smaller Company**
- [ ] Run `/company-research`
- [ ] Input: "Linear"
- [ ] Verify output still provides useful info

**Test 3: Obscure Company (Fallback Test)**
- [ ] Run `/company-research`
- [ ] Input: A small startup with limited online presence
- [ ] Verify: If web search fails, asks for links/URLs

**Test 4: With Role Specified**
- [ ] Run `/company-research`
- [ ] Input: "Stripe" for "Design Systems Engineer"
- [ ] Verify output tailors talking points to that specific role

---

### /interview-prep

**Test 1: Phone Screen**
- [ ] Run `/interview-prep`
- [ ] Input: Linear, Senior Product Designer, phone screen
- [ ] Verify output includes:
  - [ ] Likely questions based on JD
  - [ ] Talking points with specific projects
  - [ ] Short portfolio presentation guidance (appropriate for phone screen)
  - [ ] Questions to ask them

**Test 2: Portfolio Review**
- [ ] Run `/interview-prep`
- [ ] Input: Same role, but "portfolio review" stage
- [ ] Verify output:
  - [ ] More detailed portfolio presentation guidance
  - [ ] Which 2-3 case studies to present
  - [ ] Time allocation per case study
  - [ ] What to emphasize vs skip

**Test 3: Onsite**
- [ ] Run `/interview-prep`
- [ ] Input: Same role, but "onsite" stage
- [ ] Verify output covers:
  - [ ] Different question types (behavioral, portfolio, whiteboard)
  - [ ] Multiple interviewers consideration
  - [ ] Full-day preparation

**Test 4: JD Requirement Matching**
- [ ] Include "accessibility" in job description
- [ ] Verify output generates accessibility-related questions
- [ ] Verify talking points reference Medley accessibility work

---

### /thank-you

**Test 1: Standard Follow-Up**
- [ ] Run `/thank-you`
- [ ] Input: "Sarah Chen, Design Lead" / "We discussed the dashboard project and design systems"
- [ ] Verify output:
  - [ ] 4-6 sentences
  - [ ] References specific topic discussed
  - [ ] No "Thank you for your time" (generic)
  - [ ] No "I really enjoyed our conversation" (empty)
  - [ ] Has subject line

**Test 2: Addressing a Concern**
- [ ] Run `/thank-you`
- [ ] Input: Add concern: "She asked about my experience with fast-paced environments and seemed hesitant"
- [ ] Verify output addresses this concern directly

**Test 3: With Follow-Up Offer**
- [ ] Run `/thank-you`
- [ ] Input: "We discussed a tricky mobile navigation problem"
- [ ] Verify output offers to share additional thoughts/sketch

**Test 4: Uses Correct Name**
- [ ] Verify email is signed with name from resume.md (Sarah Chen)
- [ ] Verify tone matches writing-style.md preferences

---

## Edge Case Tests

### Error Handling
- [ ] Run skill and immediately send empty input — should prompt again
- [ ] Run `/cover-letter` with very short JD (1 sentence) — should still work or ask for more
- [ ] Run `/application-answer` with gibberish question — should handle gracefully

### Tone Consistency
- [ ] Run 3 different skills in sequence
- [ ] Verify tone is consistent across all outputs (matches writing-style.md)

### Context Updates
- [ ] Change a project name in portfolio.md
- [ ] Run a skill — verify it uses the new name
- [ ] (Tests that context files are re-read each time)

---

## Output Quality Checks

For each skill output, verify:
- [ ] No "leverage," "synergy," "utilize," or other AI-giveaway words
- [ ] No excessive em dashes (max 1-2 per output)
- [ ] No "I am writing to express my interest..."
- [ ] No "I hope this finds you well"
- [ ] Sentence length varies (not all same length)
- [ ] Has personality (not robotic)
- [ ] References real projects by name
- [ ] Includes metrics where appropriate

---

## Final Checks

- [ ] All 6 skills run without errors
- [ ] All skills read context files correctly
- [ ] Placeholder detection works (prompts for info when needed)
- [ ] Output quality is consistent
- [ ] No obvious bugs or crashes

---

## Notes

Record any issues found during testing:

| Skill | Issue | Severity | Fixed? |
|-------|-------|----------|--------|
| | | | |
| | | | |
| | | | |

---

## Sign-Off

- [ ] All tests passed
- [ ] Issues documented and fixed
- [ ] Ready for launch

Tested by: ________________
Date: ________________
