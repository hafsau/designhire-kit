# Resume Tailor

Customize your resume for a specific job, optimizing for ATS systems and hiring manager attention.

## Usage

```
/resume-tailor
```

Then paste the job description.

## What It Does

1. Reads your master resume from `context/resume.md`
2. Analyzes the job description for keywords and priorities
3. Reorders experience to lead with what's most relevant
4. Adjusts language to mirror job description (ATS optimization)
5. Emphasizes metrics that match their priorities
6. Outputs a tailored resume for that specific role

## Key Stats (2025 Data)

- **ATS systems filter 75% of resumes** before human review
- **6-7 seconds** — average time hiring managers spend on initial scan
- **60-75% keyword match** needed to pass ATS filters
- Tailored resumes get **3x more callbacks** than generic ones

## Instructions for Claude

When the user runs `/resume-tailor`:

### Phase 1: Context Gathering

1. Read the user's master resume:
   - `context/resume.md` for their full experience

2. **Check if resume is filled in.** If it contains placeholder text, ask the user to either:
   - Fill in the context file first, OR
   - Paste their current resume directly

3. Ask the user to paste the job description.

### Phase 2: Job Analysis

4. Analyze the job description for:
   - **Must-have skills** (required qualifications)
   - **Nice-to-have skills** (preferred qualifications)
   - **Keywords to mirror** (exact phrases they use)
   - **Priorities** (what they emphasize most)
   - **Company stage** (startup vs enterprise — affects tone)
   - **Design focus** (product, UX, visual, systems, etc.)

5. Identify keyword categories:
   - Tools: Figma, Sketch, Prototyping, etc.
   - Methods: User research, Design systems, A/B testing, etc.
   - Soft skills: Collaboration, Communication, Leadership, etc.
   - Domain: B2B, Consumer, Healthcare, Fintech, etc.

### Phase 3: Resume Optimization

6. Reorder experience sections:
   - **Lead with most relevant role** (not necessarily most recent)
   - Move relevant projects/bullets to top of each section
   - If they mention specific skills, ensure those appear early

7. Mirror exact language:
   - Use their exact phrases where authentic (ATS matching)
   - Example: If they say "design systems," use that exact phrase (not "component libraries")
   - Include both acronyms AND full terms: "UX (User Experience)"

8. Emphasize matching metrics:
   - If they want "business impact" → lead with revenue/conversion metrics
   - If they want "user focus" → lead with user satisfaction/research metrics
   - If they want "scale" → emphasize team size, user base, system scope

9. Adjust or minimize:
   - De-emphasize irrelevant experience (but don't remove — gaps look bad)
   - Shorten descriptions of less-relevant roles
   - Remove outdated tools/skills unless they're listed

### Phase 4: ATS Optimization

10. Apply ATS best practices:
    - Use standard section headers: "Experience," "Skills," "Education"
    - No tables, columns, or graphics (describe visually if needed)
    - Include exact job title if you've held it (or close variant)
    - Add skills section with keyword list

11. Format for scanning:
    - Most important info in first 1/3 of resume
    - Quantified achievements in bullet points
    - Action verbs: Led, Designed, Shipped, Reduced, Increased

### Phase 5: Output

12. Output the tailored resume with:
    - Clear section headers
    - Highlighted changes (what was reordered/adjusted)
    - Keyword match summary
    - Any warnings (missing required skills, etc.)

### Phase 6: Recruiter Review (Built-In Evaluation)

13. **Put on your senior recruiter hat** and evaluate the resume:
    - Do a 6-second scan — what's the first impression?
    - Identify strengths that would make you want to interview
    - Flag red flags or concerns a recruiter would have
    - Give a verdict: STRONG FIT / GOOD FIT / WEAK FIT / NOT A FIT
    - Provide specific recommendation to strengthen before sending

This evaluation should be honest and critical — it's better to catch issues now than after sending.

## Output Format

```
# [Name] — [Tailored Title That Matches JD]

## Summary
[2-3 sentences positioning you for THIS specific role]

## Experience

### [Most Relevant Role First]
**[Company]** | [Dates]
- [Most relevant achievement with metric]
- [Second relevant achievement]
- [Third achievement]

### [Second Role]
...

## Skills
[Keywords from job description that you actually have]

## Education
[If relevant]

---

## Optimization Notes

**Keywords matched:** [X of Y required keywords]
- [List of matched keywords]

**Keywords missing:**
- [Any required keywords you don't have — be honest]

**Changes made:**
- Reordered [X] to lead based on their emphasis on [Y]
- Added keyword "[Z]" to match their language
- Emphasized [metric type] based on their priorities

**Warnings:**
- [Any gaps or concerns to address in cover letter]

---

## Recruiter Review

**Putting on my senior recruiter hat (10+ years hiring designers):**

**First Impression (6-second scan):**
[What stands out? What's confusing? Would I keep reading?]

**Strengths:**
- [What makes this candidate compelling for THIS role]
- [What would make me want to interview them]

**Red Flags / Concerns:**
- [What might make me hesitate]
- [What questions would I have]

**Verdict:** [STRONG FIT / GOOD FIT / WEAK FIT / NOT A FIT]

**Recommendation:** [Specific suggestion to strengthen before sending]
```

## Example

**Job Description emphasis:** Design systems, cross-functional collaboration, B2B SaaS

**Original resume order:**
1. Current role at healthcare startup
2. Previous role at agency
3. Design system work at tech company

**Tailored resume order:**
1. Design system work at tech company (most relevant)
2. Current role at healthcare startup (B2B experience)
3. Previous role at agency (shortened)

**Language adjustments:**
- "Component library" → "Design system" (their language)
- Added "cross-functional" to collaboration descriptions
- Emphasized B2B metrics over consumer metrics

## What NOT to Do

- **Don't lie** — never add skills or experience you don't have
- **Don't remove jobs** — gaps raise red flags; just shorten irrelevant ones
- **Don't keyword stuff** — ATS catches unnatural repetition
- **Don't change job titles** — unless variant is accurate and matches better
- **Don't use graphics/tables** — ATS can't parse them

## When Experience Doesn't Match

If the user lacks required experience:

1. **Find transferable parallels** — "I haven't done fintech, but healthcare has similar compliance constraints"

2. **Be honest in output** — Flag missing keywords so they can address in cover letter

3. **Emphasize adjacent skills** — If they want "design systems" and user has "component library work," that's close

4. **Suggest what to highlight** — "Your [X] experience is the closest match — lead with that"

## Quality Checks

Before outputting:

- [ ] Does the summary directly address what they're looking for?
- [ ] Are the most relevant experiences at the top?
- [ ] Do bullet points include metrics?
- [ ] Are their exact keywords present (where authentic)?
- [ ] Is it ATS-friendly (no tables, standard headers)?
- [ ] Is it 1-2 pages max?
- [ ] Did I flag any missing required skills?

## Notes

- **One resume per application** — generic resumes get filtered out
- **Summary is critical** — it's the first thing humans read after ATS
- **Metrics matter** — quantify everything possible
- **Mirror their language** — ATS looks for exact keyword matches
- **Don't overthink formatting** — clean and scannable beats creative
- **Address gaps in cover letter** — resume flags them, cover letter explains
